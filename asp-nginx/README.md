  log_format access
        '{"version": "2", '
        '"time": "$time_iso8601", '
        '"remote_addr": "$remote_addr", '
        '"status": "$status", '
        '"bytes_sent": "$bytes_sent", '
        '"host": "$host", '
        '"request_method": "$request_method", '
        '"request_uri": "$request_uri", '
        '"request_time": "$request_time", '
        '"http_referer": "$http_referer", '
        '"body_bytes_sent": "$body_bytes_sent", '
        '"http_user_agent": "$http_user_agent", '
        '"http_x_forwarded_for": "$http_x_forwarded_for", '
        '"coohua_id": "$http_coohua_id", '
        '"ukey": "$http_u_key", '
        '"vkey": "$http_v_key", '
        '"upstream_ip": "$upstream_addr",'
        '"response_time": "$upstream_response_time",'
        '"cookie": "$http_cookie"}';

    access_log  /data/coohua/logs/nginx/access.log  access;
