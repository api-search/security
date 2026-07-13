---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: prestigeconsumerhealthcare.com
  spf: false
hosts:
- cert_expires: Oct  9 06:37:58 2026 GMT
  host: www.prestigeconsumerhealthcare.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 07:01:14 2026 GMT
  host: developer.prestigeconsumerhealthcare.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 07:01:14 2026 GMT
  host: api.prestigeconsumerhealthcare.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prestige Consumer Healthcare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prestige Consumer Healthcare, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Prestige Consumer Healthcare
provider_slug: prestige-consumer-healthcare
slug: prestige-consumer-healthcare-domain-security
source_filename: prestige-consumer-healthcare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.prestigeconsumerhealthcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 06:37:58 2026 GMT\n  hsts: null\n- host: developer.prestigeconsumerhealthcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 07:01:14 2026 GMT\n  hsts: null\n- host: api.prestigeconsumerhealthcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 07:01:14 2026 GMT\n  hsts: null\ndomains:\n- domain: prestigeconsumerhealthcare.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prestige-consumer-healthcare/refs/heads/main/security/prestige-consumer-healthcare-domain-security.yml
summary_line: TLSv1.3
tags:
- Consumer Healthcare
- OTC
---
