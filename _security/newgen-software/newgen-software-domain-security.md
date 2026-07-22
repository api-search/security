---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: newgensoft.com
  spf: true
hosts:
- host: www.newgensoft.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Newgen Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Newgen Software, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Newgen Software
provider_slug: newgen-software
slug: newgen-software-domain-security
source_filename: newgen-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.newgensoft.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: newgensoft.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newgen-software/refs/heads/main/security/newgen-software-domain-security.yml
summary_line: DMARC
tags:
- Company
- Saas
- Low-Code
- Content Management
- Business Process Management
- Customer Communication Management
- Document Management
- Intelligent Document Processing
- Workflow Automation
- Enterprise Software
- Digital Transformation
---
