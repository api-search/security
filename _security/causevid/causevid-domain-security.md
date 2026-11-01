---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: causevid.com
  spf: true
hosts:
- host: causevid.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1127)'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Causevid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CauseVid, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: CauseVid
provider_slug: causevid
slug: causevid-domain-security
source_filename: causevid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: causevid.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1127)'\n  hsts: null\ndomains:\n- domain: causevid.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/causevid/security/causevid-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Nonprofit
- Video
- Fundraising
- Marketing
- SaaS
---
