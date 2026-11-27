---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: agentstamp.org
  spf: true
hosts:
- cert_expires: Dec  3 16:36:01 2026 GMT
  host: agentstamp.org
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: agentstamp-org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for agentstamp-org, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: agentstamp-org
provider_slug: agentstamp-org
slug: agentstamp-org-domain-security
source_filename: agentstamp-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentstamp.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 16:36:01 2026 GMT\n  hsts: null\ndomains:\n- domain: agentstamp.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/agentstamp-org/security/agentstamp-org-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
