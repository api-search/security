---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1; p=quarantine; pct=25; rua=mailto:netadmin@linear.com
  dnssec: false
  domain: linear.com
  role: legacy
  spf: true
  spf_record: v=spf1 ip4:67.216.78.8 ip4:64.57.218.70 ip4:64.106.227.8 ip4:52.36.127.245 ip4:64.89.44.0/23 ip4:167.216.128.0/22 ip4:207.211.31.0/25 ip4:54.235.159.97 include:servers.mcsv.net include:spf-00123c01.pphosted.com include:_spf.google.com ip4:12.218.215.72 ip4:38.111.151.72 ~all
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: analog.com
  role: successor
  spf: true
hosts:
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: www.linear.com
  hsts: null
  http_status: 301
  https: true
  redirects_to: https://www.analog.com
  role: legacy-primary
  tls_version: TLSv1.3
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: linear.com
  hsts: null
  http_status: 301
  https: true
  redirects_to: https://www.linear.com/
  role: legacy-apex
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: www.analog.com
  hsts: null
  https: true
  role: successor-redirect-target
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Linear Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Linear Technology, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Linear Technology
provider_slug: linear-technology
slug: linear-technology-domain-security
source_filename: linear-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of linear.com (the entity's own domain) and its redirect target\nnote: Linear Technology was acquired by Analog Devices (closed 2017-03-10). The linear.com domain is still\n  registered and resolving, but is operated by Analog Devices and permanently redirects. Both the legacy\n  domain and the redirect target are recorded, and labeled, so the successor's posture is never mistaken\n  for this entity's own.\nhosts:\n- host: www.linear.com\n  role: legacy-primary\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\n  http_status: 301\n  redirects_to: https://www.analog.com\n- host: linear.com\n  role: legacy-apex\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: null\n  http_status: 301\n  redirects_to: https://www.linear.com/\n- host: www.analog.com\n  role: successor-redirect-target\n  https: true\n  tls_version: TLSv1.3\n\
  \  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: linear.com\n  role: legacy\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 ip4:67.216.78.8 ip4:64.57.218.70 ip4:64.106.227.8 ip4:52.36.127.245 ip4:64.89.44.0/23\n    ip4:167.216.128.0/22 ip4:207.211.31.0/25 ip4:54.235.159.97 include:servers.mcsv.net include:spf-00123c01.pphosted.com\n    include:_spf.google.com ip4:12.218.215.72 ip4:38.111.151.72 ~all\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_record: 'v=DMARC1; p=quarantine; pct=25; rua=mailto:netadmin@linear.com'\n- domain: analog.com\n  role: successor\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nwell_known_probes:\n  note: Probed on the entity's own host. No well-known document is served; every path returns a permanent\n    redirect to the Analog Devices \"ADI + Linear combine\" landing page. Absence is valid, expected data\n    for an acquired company.\n  host: https://www.linear.com\n  redirect_target:\
  \ https://www.analog.com/en/landing-pages/001/adi-linear-combine/index.html?source=ltc\n  results:\n  - path: /.well-known/security.txt\n    status: 301\n    found: false\n  - path: /.well-known/openid-configuration\n    status: 301\n    found: false\n  - path: /.well-known/oauth-authorization-server\n    status: 301\n    found: false\n  - path: /.well-known/api-catalog\n    status: 301\n    found: false\n  - path: /.well-known/ai-plugin.json\n    status: 301\n    found: false\n  - path: /llms.txt\n    status: 301\n    found: false\n  - path: /openapi.json\n    status: 301\n    found: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linear-technology/refs/heads/main/security/linear-technology-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Hardtech
- Semiconductor
- Analog
- Integrated Circuits
- Power Management
- Acquired
---
