---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vridhihomefinance.com
  spf: true
hosts:
- host: vridhihomefinance.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Vridhihomefinance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vridhi Home Finance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vridhi Home Finance
provider_slug: vridhihomefinance
slug: vridhihomefinance-domain-security
source_filename: vridhihomefinance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vridhihomefinance.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: vridhihomefinance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vridhihomefinance/refs/heads/main/security/vridhihomefinance-domain-security.yml
summary_line: DMARC
tags:
- Company
- Financial Services
- Housing Finance
- Home Loans
- Mortgage
- Lending
- Fintech
- India
---
