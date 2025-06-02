============
Installation
============

Navground, ROS2, and navground_ros support Linux, macOS and Windows.

Navground
=========

Follow the `documentation <https://idsia-robotics.github.io/navground/installation/index.html>`_ to install navground. This plugin does only depends on the navground_core and navground_sim C++ shared libraries.

You can install navground from source or install pre-build binaries.

Once installed, will need to source the environment to find navground

.. tabs::

   .. tab:: macOS

      .. code-block:: console

         $ . <navground_install>/setup.zsh

   .. tab:: Linux

      .. code-block:: console
         
         $ . <navground_install>install/setup.bash


   .. tab:: Windows

      .. code-block:: console
        
         $ <navground_install>install\setup.bat

where ``<navground_install>`` is the directory where you installed navground (e.g., ``/opt/navground/`` on Linux and macOS and ``C:\Program Files\navground`` in Windows).

ROS2
====

Follow the `installation instructions <https://docs.ros.org/en/jazzy/Installation.html>`_ to install a supported version of ROS2.


Navground-ROS
=============

Clone this repository in your colcon workspace and run

.. code-block:: console

   colcon build --merge-install --cmake-args -DCMAKE_BUILD_TYPE=Release --packages-select navground_ros

.. note::

   When installing from source, you are free to build navground in the same colcon workspace or in a separate location, provided you source the environment.