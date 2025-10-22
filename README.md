gpadmin@MOS-S-SGLVTST09:~$ pg_ldap_sync -c ~/arenadata_configs/ldap_config.yaml -vv -t
Traceback (most recent call last):
        22: from /usr/bin/pg_ldap_sync:23:in `<main>'
        21: from /usr/bin/pg_ldap_sync:23:in `load'
        20: from /opt/ruby/lib64/ruby/gems/2.7.0/gems/pg-ldap-sync-0.5.0/exe/pg_ldap_sync:6:in `<top (required)>'
        19: from /opt/ruby/lib64/ruby/gems/2.7.0/gems/pg-ldap-sync-0.5.0/lib/pg_ldap_sync/application.rb:434:in `run'
        18: from /opt/ruby/lib64/ruby/gems/2.7.0/gems/pg-ldap-sync-0.5.0/lib/pg_ldap_sync/application.rb:384:in `start!'
        17: from /opt/ruby/lib64/ruby/gems/2.7.0/gems/pg-ldap-sync-0.5.0/lib/pg_ldap_sync/application.rb:58:in `search_ldap_users'
        16: from /opt/ruby/lib64/ruby/gems/2.7.0/gems/net-ldap-0.19.0/lib/net/ldap.rb:777:in `search'
        15: from /opt/ruby/lib64/ruby/gems/2.7.0/gems/net-ldap-0.19.0/lib/net/ldap.rb:1283:in `paged_searches_supported?'
        14: from /opt/ruby/lib64/ruby/gems/2.7.0/gems/net-ldap-0.19.0/lib/net/ldap.rb:1217:in `search_root_dse'
        13: from /opt/ruby/lib64/ruby/gems/2.7.0/gems/net-ldap-0.19.0/lib/net/ldap.rb:784:in `search'
        12: from /opt/ruby/lib64/ruby/gems/2.7.0/gems/net-ldap-0.19.0/lib/net/ldap/instrumentation.rb:19:in `instrument'
        11: from /opt/ruby/lib64/ruby/gems/2.7.0/gems/net-ldap-0.19.0/lib/net/ldap.rb:785:in `block in search'
        10: from /opt/ruby/lib64/ruby/gems/2.7.0/gems/net-ldap-0.19.0/lib/net/ldap.rb:1311:in `use_connection'
         9: from /opt/ruby/lib64/ruby/gems/2.7.0/gems/net-ldap-0.19.0/lib/net/ldap/connection.rb:277:in `bind'
         8: from /opt/ruby/lib64/ruby/gems/2.7.0/gems/net-ldap-0.19.0/lib/net/ldap/instrumentation.rb:19:in `instrument'
         7: from /opt/ruby/lib64/ruby/gems/2.7.0/gems/net-ldap-0.19.0/lib/net/ldap/connection.rb:280:in `block in bind'
         6: from /opt/ruby/lib64/ruby/gems/2.7.0/gems/net-ldap-0.19.0/lib/net/ldap/auth_adapter/simple.rb:23:in `bind'
         5: from /opt/ruby/lib64/ruby/gems/2.7.0/gems/net-ldap-0.19.0/lib/net/ldap/connection.rb:203:in `queued_read'
         4: from /opt/ruby/lib64/ruby/gems/2.7.0/gems/net-ldap-0.19.0/lib/net/ldap/connection.rb:235:in `read'
         3: from /opt/ruby/lib64/ruby/gems/2.7.0/gems/net-ldap-0.19.0/lib/net/ldap/instrumentation.rb:19:in `instrument'
         2: from /opt/ruby/lib64/ruby/gems/2.7.0/gems/net-ldap-0.19.0/lib/net/ldap/connection.rb:236:in `block in read'
         1: from /opt/ruby/lib64/ruby/gems/2.7.0/gems/net-ldap-0.19.0/lib/net/ber/ber_parser.rb:169:in `read_ber'
/opt/ruby/lib64/ruby/gems/2.7.0/gems/net-ldap-0.19.0/lib/net/ber/ber_parser.rb:169:in `getbyte': Connection reset by peer @ io_fillbuf - fd:5  (Errno::ECONNRESET)



CN=Мишагин Кирилл Евгеньевич(MishaginKE),OU=Users,OU=PolyusDigital,OU=Krasnoyarsk,OU=Root,DC=polyus,DC=com,mos-s-dc01.polyus.com [MOS-S-DC01.polyus.com]
