.. _bt_non_blocking_sequence_control:

NonblockingSequence
===================

Ticks all child nodes until they all return SUCCESS. If any of the child nodes return RUNNING, it will continue to tick the subsequent nodes. This node will once again tick through all the child nodes if it is ticked itself. If at any time a child returns FAILURE, that stops all children and returns FAILURE overall.

For additional details regarding the ``NonblockingSequence`` please see the guide for `Nav2 Specific BT Nodes <../../../../behavior_trees/overview/nav2_specific_nodes.html>`_.

Example
-------

.. code-block:: xml

    <NonblockingSequence>
        <!--Add tree components here--->
    </NonblockingSequence>
