---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: asig.gov.al
  spf: true
hosts:
- host: asig.gov.al
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1127)'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: State Authority For Geospatial Information Asig Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for State Authority for Geospatial Information (ASIG), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: State Authority for Geospatial Information (ASIG)
provider_slug: state-authority-for-geospatial-information-asig
slug: state-authority-for-geospatial-information-asig-domain-security
source_filename: state-authority-for-geospatial-information-asig-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: asig.gov.al\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1127)'\n  hsts: null\ndomains:\n- domain: asig.gov.al\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/state-authority-for-geospatial-information-asig/security/state-authority-for-geospatial-information-asig-domain-security.yml
summary_line: DMARC
tags:
- Company
---
