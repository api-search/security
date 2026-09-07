---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: accropeutics.com
  spf: true
hosts:
- host: www.accropeutics.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Accrobioscience Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Accro Bioscience, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Accro Bioscience
provider_slug: accrobioscience
slug: accrobioscience-domain-security
source_filename: accrobioscience-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: >-\n  www.accropeutics.com negotiates TLSv1.3 but serves an INCOMPLETE certificate chain: the origin\n  presents only the leaf (CN=accropeutics.com, issued by Certum Domain Validation CA SHA2) and\n  omits the intermediate, so `openssl s_client` returns verify code 21, \"unable to verify the first\n  certificate\". Ordinary browsers recover via AIA fetching; strict clients — curl without -k,\n  Python urllib, and most server-side HTTP libraries — fail the handshake outright. The apex\n  publishes SPF but no DMARC record, no CAA records, and the accropeutics.com zone is not\n  DNSSEC-signed.\nhosts:\n- host: www.accropeutics.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: accropeutics.com\n  dnssec: false\n  caa: []\n  spf: true\n\
  \  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accrobioscience/refs/heads/main/security/accrobioscience-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Drug Discovery
- Clinical Trials
- Life Sciences
- Immunology
- Inflammation
- Small Molecule
- Regulated Cell Death
---
