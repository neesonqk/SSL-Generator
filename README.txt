Generate SSl CA, Server Certs, Client Certs
=======

Defaults:
a. valid for 100 years.
b. SHA256
c. 4096


1. Set up CA
sh setup_ca.sh RabbitSSL  # RabbitSSL 签发机构名称

2. Make server certs
sh make_server_cert.sh rabbit-server rabbit # rabbit-server 生成密匙前缀名称，自定义。 rabbit 访问该密匙的密码 

3. Create client certs
create_client_cert.sh rabbit-client rabbit # rabbit-client 生成密匙前缀名称，自定义。 rabbit 访问该密匙的密码 