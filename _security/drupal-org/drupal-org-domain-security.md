---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: drupal.org
  spf: true
hosts:
- cert_expires: Feb 18 21:00:17 2027 GMT
  host: www.drupal.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Drupal Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Drupal.org, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Drupal.org
provider_slug: drupal-org
slug: drupal-org-domain-security
source_filename: drupal-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.drupal.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 18 21:00:17 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: drupal.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drupal-org/refs/heads/main/security/drupal-org-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Open Source Projects
- Public APIs
---
