.. code-block:: csharp

.. code-block:: java

.. code-block:: javascript

.. code-block:: php

    $policy->execute();

.. code-block:: python

    # After authenticating
    au = pyrax.autoscale
    au.execute_policy("{scalingGroupId}", "{policyId}")

.. code-block:: ruby

  my_policy.execute

.. code-block:: sh

  $ curl -X POST -H "X-Auth-Token: $TOKEN" \
    $ENDPOINT/groups/{groupId}/policies/{policyId}/execute
