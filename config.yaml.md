```
listen: :443

tls:
  cert: /root/cert/fullchain.cer 
  key: /root/cert/acstudycn.eu.org.key

quic:
  initStreamReceiveWindow: 16777216
  maxStreamReceiveWindow: 16777216
  initConnReceiveWindow: 33554432
  maxConnReceiveWindow: 33554432

auth:
  type: password
  password: acstudycn

masquerade:
  type: proxy
  proxy:
    url: https://sb.scorecardresearch.com
    rewriteHost: true
```

