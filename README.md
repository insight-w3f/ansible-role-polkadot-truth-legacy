polkadot_truth_node
=========

This role transforms a Polkadot library node into a source of truth node and prepares it for S3 sync.

Requirements
------------

This package requires that you have previously prepared the instance with the insight_w3f.polkadot_library role.

Role Variables
--------------

- region: The AWS region where the S3 bucket is deployed
- aws_access_key_id: The AWS access key ID for the authorized sync user
- aws_secret_access_key: The AWS secret access key for the authorized sync user
- sync_bucket_uri: The name of the S3 bucket

Dependencies
------------

- insight_w3f.polkadot_library

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

Apache 2.0

Author Information
------------------

Maintained by [Richard Mah](https://github.com/shinyfoil) for [Insight Infrastructure](https://github.com/insight-infrastructure)