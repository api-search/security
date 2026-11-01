---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: circlehealth.co.uk
  spf: true
hosts:
- host: www.circlehealth.co.uk
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1127)'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Circlehealth Co Uk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for circlehealth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: circlehealth
provider_slug: circlehealth-co-uk
slug: circlehealth-co-uk-domain-security
source_filename: circlehealth-co-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.circlehealth.co.uk\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1127)'\n  hsts: null\ndomains:\n- domain: circlehealth.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/circlehealth-co-uk/security/circlehealth-co-uk-domain-security.yml
summary_line: DMARC
tags:
- Company
---
