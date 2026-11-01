---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: luxinnovation.lu
  spf: true
hosts:
- host: clustermembers.luxinnovation.lu
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''clustermemb'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rss Hydro Sarl S Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RSS-Hydro Sarl-S, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: RSS-Hydro Sarl-S
provider_slug: rss-hydro-sarl-s
slug: rss-hydro-sarl-s-domain-security
source_filename: rss-hydro-sarl-s-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clustermembers.luxinnovation.lu\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''clustermemb'\n  hsts: null\ndomains:\n- domain: luxinnovation.lu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/rss-hydro-sarl-s/security/rss-hydro-sarl-s-domain-security.yml
summary_line: DMARC
tags:
- Company
---
