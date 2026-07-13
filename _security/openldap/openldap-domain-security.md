---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openldap.org
  spf: true
hosts:
- cert_expires: Aug 11 11:19:45 2026 GMT
  host: www.openldap.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openldap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenLDAP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenLDAP
provider_slug: openldap
slug: openldap-domain-security
source_filename: openldap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openldap.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 11:19:45 2026 GMT\n  hsts: false\ndomains:\n- domain: openldap.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openldap/refs/heads/main/security/openldap-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Directory Services
- LDAP
- Identity
- Authentication
- Open Source
- Infrastructure
---
