Phases of Integration
=====================

.. _Phase 1 - Data Collection:

Phase 1 - Data Collection
-------------------------

This phase begins the moment a customer signs a contract. ATLAS requests the following items to ease transition through later technical phases:

.. list-table::
    :widths: 10 35 10 10
    :header-rows: 1

    * - Step
      - Description
      - Reading
      - Owner
    * - 1.1
      - | Define the Modes of Operation and technical requirements. The MOO represents the customer's 
        | desired ConOps based on the capabilities of the spacecraft. It primarily answers the questions:
        | For each mode of Operation...
        * What frequency band(s) are used?
        * What link type(s) are used (Transmit, Receive, or Both)?
        * What are the signal characteristics? I.e. modulation(s), data rate(s), polarization(s)
        * How will the data be deliverd (real time and/or store & forward)
        * What baseband equipment wil lbe used? Is header translation required?
        * What property overrides must be applied?
        * Is customer post processing required?
        * What is the data delivery destination? (ATLAS S3 or push to customer server)
      - :doc:`Partner Communications`
      - ATLAS
    * - 1.2
      - | For each Mode of Operation, ATLAS needs representative **Downlink** Data File(s)

        | This file will be used to validate telemetry output from the modem through the FPS. It can be 
        | with any header format (Cortex, Amergint, RT Logic) as long as we have a description of the header
        | format available (Either supplied by the Customer or available to ATLAS)
      - 
      - Customer
    * - 1.3
      - | For each Mode of Operation, ATLAS needs representative **Uplink** Data File(s)

        | This file will be used to validate commands going through the FPS and into the modem at the site.
      - 
      - Customer

.. _Phase 2 - API Integration:

Phase 2 - API Integration
-------------------------

The API Integration Phase is to accomplish early integration and familiarity with the ATLAS Freedom API. We expect that at the end of this phase the customer understands the API and can execute the following objectives:

.. list-table::
   :widths: 10 35 10 10
   :header-rows: 1

   * - Step
     - Description
     - Reading
     - Owner
   * - 2.1
     - Create, Retrieve, and Delete **Satellite Bands**
     - :ref: '<Adding Satellites>':
     - Customer


.. _Phase 3 - Testing / Hardware Configuration:

Phase 3 - Testing / Hardware Configuration
------------------------------------------

.. _Phase 4 - AIB Compatibility Testing:

Phase 4 - AIB Compatibility Testing
-----------------------------------

.. _Phase 5 - Production:

Phase 5 - Production
--------------------