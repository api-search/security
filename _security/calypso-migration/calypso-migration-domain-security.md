---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: calypso.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nasdaq.com
  spf: true
hosts:
- host: www.calypso.com
  https: false
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: www.nasdaq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Calypso Migration Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Calypso Migration, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Calypso Migration
provider_slug: calypso-migration
slug: calypso-migration-domain-security
source_filename: calypso-migration-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.calypso.com\n  https: false\n- host: www.nasdaq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: calypso.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: nasdaq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calypso-migration/refs/heads/main/security/calypso-migration-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Capital Markets
- Data Migration
- Financial Technology
- Migration
- Trading
---
