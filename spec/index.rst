Spec Home
=========

The place where all specs lives.


Project Specs
-------------

Quick Marts (ADQM)
^^^^^^^^^^^^^^^^^^

======= ============================================================== ==========
Project Bundle                                                         ClickHouse
======= ============================================================== ==========
TBD     `adcm_cluster_adqm <https://spec.adsw.io/adcm_cluster_adqm/>`_ TBD
======= ============================================================== ==========

Second Storage (ADSS)
^^^^^^^^^^^^^^^^^^^^^

TBD

How to write specs
------------------

Quick start
^^^^^^^^^^^

* create spec dir in your repo
* go to spec dir and do the following (tested on linux only)

.. code-block:: sh

   docker run -it --rm -v $(pwd):/spec -u $(id -u ${USER}):$(id -g ${USER})  ci.arenadata.io/sphinx-autobuild /script/create_tmpl.sh

* run autobuild server with command

.. code-block:: sh

  docker run -it --rm -v $(pwd):/spec -p 9000:9000 ci.arenadata.io/sphinx-autobuild:latest

* open browser at `<http://127.0.0.1:9000>`_
* open index.rst with your favorit editor ( vim :)  and start to edit
* see changes in browser

More information about syntax in `official docs <https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html#literal-blocks>`_

More information about autobuild image in `sphinx-autobuild readme <https://github.com/arenadata/sphinx_builder>`_
