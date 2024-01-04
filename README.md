## multi-mint

casper-client put-deploy -n http://localhost:11101/rpc \
--chain-name "casper-net-1" \
--payment-amount 7500000000 \
-k /home/jh/casper-node/utils/nctl/assets/net-1/users/user-1/secret_key.pem \
--session-package-hash hash-0b13427be2c9a648358eee62ab34f818e6d4195e7686368aa335f80fa16cdeae \
--session-entry-point "multi_mint" \
--session-args-json \
'[{"name":"multi_token_meta_data","type":{"List":"String"},"value":["{\"name\": \"John Doe\",\"token_uri\": \"https:\/\/www.barfoo1.com\",\"checksum\": \"940bffb3f2bba35f84313aa26da09ece3ad47045c6a1292c2bbd2df4ab1a55fb\"}","{\"name\": \"John Doe\",\"token_uri\": \"https:\/\/www.barfoo2.com\",\"checksum\": \"940bffb3f2bba35f84313aa26da09ece3ad47045c6a1292c2bbd2df4ab1a55fb\"}"]},{"name":"multi_token_owners","type":{"List":"Key"},"value":["account-hash-c30fba121a352c6423961f9755ce08bfdb9b6ccd4fcb3d9ea308f9fcc2e5d509","account-hash-a254c35af567541efbac1b023086cd888fbbda7664f620f810b427ad727c99ab"]}]' 
