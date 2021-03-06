
.. _junipernetworks.junos.junos_static_routes_:


*****
junipernetworks.junos.junos_static_routes
*****

**Static routes resource module**


Version added: 1.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module provides declarative management of static routes on Juniper JUNOS devices



Requirements
------------
The below requirements are needed on the local master node that executes this .

- ncclient (>=v0.6.4)
- xmltodict (>=0.12)


Parameters
----------

.. raw:: html

    <table  border=0 cellpadding=0 class="documentation-table">
        <tr>
            <th colspan="5">Parameter</th>
            <th>Choices/<font color="blue">Defaults</font></th>
                            <th>Configuration</th>
                        <th width="100%">Comments</th>
        </tr>
                    <tr>
                                                                <td colspan="5">
                    <div class="ansibleOptionAnchor" id="parameter-"></div>
                    <b>config</b>
                    <a class="ansibleOptionLink" href="#parameter-" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">list</span>
                         / <span style="color: purple">elements=dictionary</span>                                            </div>
                                    </td>
                                <td>
                                                                                                                                                            </td>
                                                    <td>
                                                                                            </td>
                                                <td>
                                            <div>A dictionary of static routes options</div>
                                                        </td>
            </tr>
                                                            <tr>
                                                    <td class="elbow-placeholder"></td>
                                                <td colspan="4">
                    <div class="ansibleOptionAnchor" id="parameter-"></div>
                    <b>address_families</b>
                    <a class="ansibleOptionLink" href="#parameter-" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">list</span>
                         / <span style="color: purple">elements=dictionary</span>                                            </div>
                                    </td>
                                <td>
                                                                                                                                                            </td>
                                                    <td>
                                                                                            </td>
                                                <td>
                                            <div>Address family to use for the static routes</div>
                                                        </td>
            </tr>
                                                            <tr>
                                                    <td class="elbow-placeholder"></td>
                                    <td class="elbow-placeholder"></td>
                                                <td colspan="3">
                    <div class="ansibleOptionAnchor" id="parameter-"></div>
                    <b>afi</b>
                    <a class="ansibleOptionLink" href="#parameter-" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">string</span>
                                                 / <span style="color: red">required</span>                    </div>
                                    </td>
                                <td>
                                                                                                                            <ul style="margin: 0; padding: 0"><b>Choices:</b>
                                                                                                                                                                <li>ipv4</li>
                                                                                                                                                                                                <li>ipv6</li>
                                                                                    </ul>
                                                                            </td>
                                                    <td>
                                                                                            </td>
                                                <td>
                                            <div>afi to use for the static routes</div>
                                                        </td>
            </tr>
                                <tr>
                                                    <td class="elbow-placeholder"></td>
                                    <td class="elbow-placeholder"></td>
                                                <td colspan="3">
                    <div class="ansibleOptionAnchor" id="parameter-"></div>
                    <b>routes</b>
                    <a class="ansibleOptionLink" href="#parameter-" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">list</span>
                         / <span style="color: purple">elements=dictionary</span>                                            </div>
                                    </td>
                                <td>
                                                                                                                                                            </td>
                                                    <td>
                                                                                            </td>
                                                <td>
                                            <div>Static route configuration</div>
                                                        </td>
            </tr>
                                                            <tr>
                                                    <td class="elbow-placeholder"></td>
                                    <td class="elbow-placeholder"></td>
                                    <td class="elbow-placeholder"></td>
                                                <td colspan="2">
                    <div class="ansibleOptionAnchor" id="parameter-"></div>
                    <b>dest</b>
                    <a class="ansibleOptionLink" href="#parameter-" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">string</span>
                                                                    </div>
                                    </td>
                                <td>
                                                                                                                                                            </td>
                                                    <td>
                                                                                            </td>
                                                <td>
                                            <div>Static route destination including prefix</div>
                                                        </td>
            </tr>
                                <tr>
                                                    <td class="elbow-placeholder"></td>
                                    <td class="elbow-placeholder"></td>
                                    <td class="elbow-placeholder"></td>
                                                <td colspan="2">
                    <div class="ansibleOptionAnchor" id="parameter-"></div>
                    <b>metric</b>
                    <a class="ansibleOptionLink" href="#parameter-" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">integer</span>
                                                                    </div>
                                    </td>
                                <td>
                                                                                                                                                            </td>
                                                    <td>
                                                                                            </td>
                                                <td>
                                            <div>Metric value for the static route</div>
                                                        </td>
            </tr>
                                <tr>
                                                    <td class="elbow-placeholder"></td>
                                    <td class="elbow-placeholder"></td>
                                    <td class="elbow-placeholder"></td>
                                                <td colspan="2">
                    <div class="ansibleOptionAnchor" id="parameter-"></div>
                    <b>next_hop</b>
                    <a class="ansibleOptionLink" href="#parameter-" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">list</span>
                         / <span style="color: purple">elements=dictionary</span>                                            </div>
                                    </td>
                                <td>
                                                                                                                                                            </td>
                                                    <td>
                                                                                            </td>
                                                <td>
                                            <div>Next hop to destination</div>
                                                        </td>
            </tr>
                                                            <tr>
                                                    <td class="elbow-placeholder"></td>
                                    <td class="elbow-placeholder"></td>
                                    <td class="elbow-placeholder"></td>
                                    <td class="elbow-placeholder"></td>
                                                <td colspan="1">
                    <div class="ansibleOptionAnchor" id="parameter-"></div>
                    <b>forward_router_address</b>
                    <a class="ansibleOptionLink" href="#parameter-" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">string</span>
                                                                    </div>
                                    </td>
                                <td>
                                                                                                                                                            </td>
                                                    <td>
                                                                                            </td>
                                                <td>
                                            <div>List of next hops</div>
                                                        </td>
            </tr>
                    
                                    
                                    
                                                <tr>
                                                    <td class="elbow-placeholder"></td>
                                                <td colspan="4">
                    <div class="ansibleOptionAnchor" id="parameter-"></div>
                    <b>vrf</b>
                    <a class="ansibleOptionLink" href="#parameter-" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">string</span>
                                                                    </div>
                                    </td>
                                <td>
                                                                                                                                                            </td>
                                                    <td>
                                                                                            </td>
                                                <td>
                                            <div>Virtual Routing and Forwarding (VRF) name</div>
                                                        </td>
            </tr>
                    
                                                <tr>
                                                                <td colspan="5">
                    <div class="ansibleOptionAnchor" id="parameter-"></div>
                    <b>state</b>
                    <a class="ansibleOptionLink" href="#parameter-" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">string</span>
                                                                    </div>
                                    </td>
                                <td>
                                                                                                                            <ul style="margin: 0; padding: 0"><b>Choices:</b>
                                                                                                                                                                <li><div style="color: blue"><b>merged</b>&nbsp;&larr;</div></li>
                                                                                                                                                                                                <li>replaced</li>
                                                                                                                                                                                                <li>overridden</li>
                                                                                                                                                                                                <li>deleted</li>
                                                                                    </ul>
                                                                            </td>
                                                    <td>
                                                                                            </td>
                                                <td>
                                            <div>The state the configuration should be left in</div>
                                                        </td>
            </tr>
                        </table>
    <br/>


Notes
-----

.. note::
   - This module requires the netconf system service be enabled on the device being managed.
   - This module works with connection ``netconf``. See `the Junos OS Platform Options <../network/user_guide/platform_junos.html>`_.
   - Tested against JunOS v18.4R1



Examples
--------

.. code-block:: yaml+jinja

    
    # Using deleted

    # Before state
    # ------------
    #
    # admin# show routing-options
    # static {
    #     route 192.168.47.0/24 next-hop 172.16.1.2;
    #     route 192.168.16.0/24 next-hop 172.16.1.2;
    #     route 10.200.16.75/24 next-hop 10.200.16.2;
    # }

    - name: Delete provided configuration (default operation is merge)
      junipernetworks.junos.junos_static_routes:
        config:
        - address_families:
          - afi: ipv4
            routes:
            - dest: 10.200.16.75/24
              next_hop:
              - forward_router_address: 10.200.16.2
        state: deleted

    # After state:
    # ------------
    #
    # admin# show routing-options
    # static {
    #     route 192.168.47.0/24 next-hop 172.16.1.2;
    #     route 192.168.16.0/24 next-hop 172.16.1.2;
    # }

    # Using merged

    # Before state
    # ------------
    #
    # admin# show routing-options
    # static {
    #     route 192.168.47.0/24 next-hop 172.16.1.2;
    #     route 192.168.16.0/24 next-hop 172.16.1.2;
    # }

    - name: Merge provided configuration with device configuration (default operation
        is merge)
      junipernetworks.junos.junos_static_routes:
        config:
        - address_families:
          - afi: ipv4
            routes:
            - dest: 10.200.16.75/24
              next_hop:
              - forward_router_address: 10.200.16.2
        state: merged

    # After state:
    # ------------
    #
    # admin# show routing-options
    # static {
    #     route 192.168.47.0/24 next-hop 172.16.1.2;
    #     route 192.168.16.0/24 next-hop 172.16.1.2;
    #     route 10.200.16.75/24 next-hop 10.200.16.2;
    # }

    # Using overridden

    # Before state
    # ------------
    #
    # admin# show routing-options
    # static {
    #     route 192.168.47.0/24 next-hop 172.16.1.2;
    #     route 192.168.16.0/24 next-hop 172.16.0.1;
    # }

    - name: Override provided configuration with device configuration (default operation
        is merge)
      junipernetworks.junos.junos_static_routes:
        config:
        - address_families:
          - afi: ipv4
            routes:
            - dest: 10.200.16.75/24
              next_hop:
              - forward_router_address: 10.200.16.2
        state: overridden

    # After state:
    # ------------
    #
    # admin# show routing-options
    # static {
    #     route 10.200.16.75/24 next-hop 10.200.16.2;
    # }

    # Using replaced

    # Before state
    # ------------
    #
    # admin# show routing-options
    # static {
    #     route 192.168.47.0/24 next-hop 172.16.1.2;
    #     route 192.168.16.0/24 next-hop 172.16.1.2;
    # }

    - name: Replace provided configuration with device configuration (default operation
        is merge)
      junipernetworks.junos.junos_static_routes:
        config:
        - address_families:
          - afi: ipv4
            routes:
            - dest: 192.168.47.0/24
              next_hop:
              - forward_router_address: 10.200.16.2
        state: replaced

    # After state:
    # ------------
    #
    # admin# show routing-options
    # static {
    #     route 192.168.47.0/24 next-hop 10.200.16.2;
    #     route 192.168.16.0/24 next-hop 172.16.1.2;
    # }






Return Values
-------------
Common return values are documented :ref:`here <common_return_values>`, the following are the fields unique to this :

.. raw:: html

    <table border=0 cellpadding=0 class="documentation-table">
        <tr>
            <th colspan="1">Key</th>
            <th>Returned</th>
            <th width="100%">Description</th>
        </tr>
                    <tr>
                                <td colspan="1">
                    <div class="ansibleOptionAnchor" id="return-"></div>
                    <b>after</b>
                    <a class="ansibleOptionLink" href="#return-" title="Permalink to this return value"></a>
                    <div style="font-size: small">
                      <span style="color: purple">string</span>
                                          </div>
                                    </td>
                <td>when changed</td>
                <td>
                                                                        <div>The resulting configuration model invocation.</div>
                                                                <br/>
                                            <div style="font-size: smaller"><b>Sample:</b></div>
                                                <div style="font-size: smaller; color: blue; word-wrap: break-word; word-break: break-all;">The configuration returned will always be in the same format
     of the parameters above.</div>
                                    </td>
            </tr>
                                <tr>
                                <td colspan="1">
                    <div class="ansibleOptionAnchor" id="return-"></div>
                    <b>before</b>
                    <a class="ansibleOptionLink" href="#return-" title="Permalink to this return value"></a>
                    <div style="font-size: small">
                      <span style="color: purple">string</span>
                                          </div>
                                    </td>
                <td>always</td>
                <td>
                                                                        <div>The configuration prior to the model invocation.</div>
                                                                <br/>
                                            <div style="font-size: smaller"><b>Sample:</b></div>
                                                <div style="font-size: smaller; color: blue; word-wrap: break-word; word-break: break-all;">The configuration returned will always be in the same format
     of the parameters above.</div>
                                    </td>
            </tr>
                                <tr>
                                <td colspan="1">
                    <div class="ansibleOptionAnchor" id="return-"></div>
                    <b>commands</b>
                    <a class="ansibleOptionLink" href="#return-" title="Permalink to this return value"></a>
                    <div style="font-size: small">
                      <span style="color: purple">list</span>
                                          </div>
                                    </td>
                <td>always</td>
                <td>
                                                                        <div>The set of commands pushed to the remote device.</div>
                                                                <br/>
                                            <div style="font-size: smaller"><b>Sample:</b></div>
                                                <div style="font-size: smaller; color: blue; word-wrap: break-word; word-break: break-all;">[&#x27;command 1&#x27;, &#x27;command 2&#x27;, &#x27;command 3&#x27;]</div>
                                    </td>
            </tr>
                        </table>
    <br/><br/>


Status
------


Authors
~~~~~~~

- Daniel Mellado (@dmellado)


.. hint::
    If you notice any issues in this documentation, you can `edit this document <https://github.com/ansible/ansible/edit/devel/lib/ansible/plugins//?description=%23%23%23%23%23%20SUMMARY%0A%3C!---%20Your%20description%20here%20--%3E%0A%0A%0A%23%23%23%23%23%20ISSUE%20TYPE%0A-%20Docs%20Pull%20Request%0A%0A%2Blabel:%20docsite_pr>`_ to improve it.


.. hint::
    Configuration entries for each entry type have a low to high priority order. For example, a variable that is lower in the list will override a variable that is higher up.
