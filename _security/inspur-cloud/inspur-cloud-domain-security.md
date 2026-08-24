---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: inspur.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: inspurcloudapi.com
  spf: false
hosts:
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: cloud.inspur.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: console1.cloud.inspur.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- host: ecs.cn-north-3.inspurcloudapi.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1129)'
kind: domain-security
layout: security
method: probed
name: Inspur Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inspur Cloud, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Inspur Cloud
provider_slug: inspur-cloud
slug: inspur-cloud-domain-security
source_filename: inspur-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloud.inspur.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: console1.cloud.inspur.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: false\n- host: ecs.cn-north-3.inspurcloudapi.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer\n    certificate (_ssl.c:1129)'\n  hsts: null\ndomains:\n- domain: inspur.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: inspurcloudapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\nfindings:\n- id: expired-api-host-certificates\n  severity: high\n  detail: The public API endpoint hosts serve TLS certificates that expired years ago. ecs.cn-north-3.inspurcloudapi.com\n\
  \    presents CN=*.cn-north-3.inspurcloudapi.com issued by TrustAsia TLS RSA CA, valid 2019-12-10 to 2020-12-09.\n    ecs.cn-east-1.inspurcloudapi.com presents CN=*.cn-east-1.inspurcloudapi.com, valid 2021-07-09 to 2022-07-08.\n    Any client performing standard certificate validation cannot complete a TLS handshake with these hosts.\n  observed: '2026-08-23'\n  hosts:\n  - ecs.cn-north-3.inspurcloudapi.com\n  - ecs.cn-east-1.inspurcloudapi.com\n- id: api-host-certificate-name-mismatch\n  severity: medium\n  detail: iam.inspurcloudapi.com resolves via iam.cn-north-3.inspurcloudapi.com to a host presenting CN=*.cloud.inspur.com\n    (sslTrus DV CA, valid 2026-02-06 to 2027-02-06) — a currently-valid certificate for a different name\n    than the API host.\n  observed: '2026-08-23'\n- id: www-inspurcloudapi-is-not-the-provider\n  severity: info\n  detail: www.inspurcloudapi.com resolves to a ChinaNetCenter/Wangsu CDN edge presenting CN=default.chinanetcenter.com\n    with SANs for unrelated\
  \ properties (4399.com, dianping.com, meituan.net). The apex inspurcloudapi.com\n    does not resolve. Only the <service>.<region>.inspurcloudapi.com names documented in the API references\n    are Inspur Cloud API hosts.\n  observed: '2026-08-23'\n- id: spf-dmarc-absent-on-api-domain\n  severity: low\n  detail: inspurcloudapi.com publishes neither SPF nor DMARC; the corporate domain inspur.com publishes\n    both, with a DMARC policy of reject.\n  observed: '2026-08-23'\napi_host_reachability:\n  probed: '2026-08-23'\n  method: direct TCP connect on 443 and 80, plus an unverified TLS handshake to read the presented certificate,\n    against every service host named in the Inspur Cloud API references\n  summary: Not one of the nine documented Inspur Cloud API endpoint hosts presents a currently-valid certificate\n    for its own name. Two refuse TCP connections entirely, four present certificates that expired between\n    2020 and 2022, one answers with a Kubernetes ingress default-backend\
  \ placeholder certificate, and\n    one presents a certificate for a different name. Only the object-storage endpoint completes a normal\n    HTTPS request.\n  hosts:\n  - host: ecs.cn-north-3.inspurcloudapi.com\n    ip: 117.73.11.33\n    tcp_443: open\n    certificate: CN=*.cn-north-3.inspurcloudapi.com, TrustAsia TLS RSA CA\n    valid_from: '2019-12-10'\n    valid_to: '2020-12-09'\n    verdict: expired 2020-12-09\n  - host: ecs.cn-east-1.inspurcloudapi.com\n    tcp_443: open\n    certificate: CN=*.cn-east-1.inspurcloudapi.com, TrustAsia TLS RSA CA\n    valid_from: '2021-07-09'\n    valid_to: '2022-07-08'\n    verdict: expired 2022-07-08\n  - host: ecs.cn-south-1.inspurcloudapi.com\n    ip: 121.46.129.183\n    tcp_443: timeout\n    verdict: unreachable from outside China (connection timed out)\n  - host: ebs.cn-north-3.inspurcloudapi.com\n    ip: 117.73.11.33\n    tcp_443: open\n    certificate: CN=*.cn-north-3.inspurcloudapi.com\n    valid_to: '2020-12-09'\n    verdict: expired 2020-12-09\n\
  \  - host: vpc.cn-north-3.inspurcloudapi.com\n    ip: 117.73.11.33\n    tcp_443: open\n    certificate: CN=*.cn-north-3.inspurcloudapi.com\n    valid_to: '2020-12-09'\n    verdict: expired 2020-12-09\n  - host: eip.cn-north-3.inspurcloudapi.com\n    ip: 117.73.11.33\n    tcp_443: open\n    certificate: CN=*.cn-north-3.inspurcloudapi.com, O=山东浪潮云服务信息科技有限公司 (Shandong Inspur Cloud Service\n      Information Technology Co., Ltd.), OU=产品中心, L=济南, ST=山东\n    valid_from: '2019-01-30'\n    valid_to: '2020-02-03'\n    verdict: expired 2020-02-03 — the oldest of the set. This is also the only certificate in the estate\n      that names the operating legal entity, which independently confirms the inspurcloudapi.com API domain\n      belongs to Inspur Cloud.\n  - host: mysql.cn-north-3.inspurcloudapi.com\n    ip: 117.73.11.33\n    tcp_443: open\n    certificate: O=Acme Co, CN=Kubernetes Ingress Controller Fake Certificate\n    valid_from: '2026-07-31'\n    valid_to: '2027-07-31'\n    verdict: no ingress\
  \ rule matches this hostname — the cluster is answering with the ingress-nginx default-backend\n      placeholder certificate, which means the documented RDS for MySQL API host is not routed\n  - host: cps.cn-north-3.inspurcloudapi.com\n    ip: 117.73.11.106\n    tcp_443: refused\n    tcp_80: refused\n    verdict: DNS resolves but nothing is listening on either port — the documented CPS API host is dead\n  - host: cbs.cn-north-3.inspurcloudapi.com\n    ip: 117.73.11.106\n    tcp_443: refused\n    tcp_80: refused\n    verdict: DNS resolves but nothing is listening on either port — the documented CBS API host is dead\n  - host: iam.inspurcloudapi.com\n    tcp_443: open\n    certificate: CN=*.cloud.inspur.com, sslTrus (RSA) DV CA\n    valid_from: '2026-02-06'\n    valid_to: '2027-02-06'\n    verdict: valid certificate for a different name — name mismatch against the documented IAM API host\n  - host: oss.cn-north-3.inspurcloudoss.com\n    ip: 117.73.1.16\n    tcp_443: open\n    verdict: the\
  \ only documented API host that completes an ordinary verified HTTPS request; returned\n      HTTP 200 with x-amz-request-id and x-amz-object-type response headers\n  consequence: Any client with default certificate validation — every SDK, every HTTP library, every agent\n    runtime — fails to connect to the compute, storage, network, identity and database APIs as documented.\n    Object Storage is the only surface an outside integrator can call without disabling verification.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inspur-cloud/refs/heads/main/security/inspur-cloud-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Cloud
- Infrastructure
- Compute
- Storage
- Networking
- Object Storage
- Identity
- Database
- Containers
- Internet of Things
- Blockchain
- China
- Company
---
