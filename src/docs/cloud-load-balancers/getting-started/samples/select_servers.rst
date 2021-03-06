.. code-block:: csharp

.. code-block:: java

.. code-block:: javascript

.. code-block:: php

  $computeService = $client->computeService('cloudServersOpenStack', 'DFW');

  // Retrieve servers using their UUIDs
  $serverOne = $computeService->server('{serverId1}');
  $serverTwo = $computeService->server('{serverId2}');

.. code-block:: python

  pyrax.connect_to_cloudservers("{region}")
  server_one = cs.servers.get('{serverId1}')
  server_two = cs.servers.get('{serverId2}')


.. code-block:: ruby

  compute = Fog::Compute.new(
    :provider => 'rackspace',
    :rackspace_username => '{username}',
    :rackspace_api_key => '{apiKey}',
    :rackspace_region => '{region}'
  )

  @server_one = compute.servers.get('{serverId1}')
  @server_two = compute.servers.get('{serverId2}')

.. code-block:: sh

  # Retrieve servers using their UUIDs.
  curl -s -X GET $COMPUTE_ENDPOINT/servers/{serverId1} \
    -H "X-Auth-Token: $TOKEN" \
    -H "Accept: application/json" | python -m json.tool

  curl -s -X GET $COMPUTE_ENDPOINT/servers/{serverId1} \
    -H "X-Auth-Token: $TOKEN" \
    -H "Accept: application/json" | python -m json.tool

  # Make a note of server.addresses.private.addr for each server.
