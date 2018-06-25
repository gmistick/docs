Snap configuration
======================

Anbox support multiple configuration and setups, you can configure the anbox system using specific flags in the snapcraft control:


Enable Anbox Debug Logs
-----------------------------

You can configure the Anbox system to write debug logs as follows:

.. code-block:: text

    $ snap set anbox debug.enable=true
    $ snap restart anbox


Running containers in privileged mode
-----------------------------

In some setups it makes sense to run the Anbox container in privileged mode, 
this can be achieved using the following commands:

.. code-block:: text

    $ snap set anbox container.privileged=true
    $ snap restart anbox.container-manager

now the container manager run with the --privileged config and will execute the containers accordingly.