---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: dataverse.org
  spf: true
hosts:
- cert_expires: Nov 16 04:13:43 2026 GMT
  host: dataverse.org
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dataverse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dataverse, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Dataverse
provider_slug: dataverse
slug: dataverse-domain-security
source_filename: dataverse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dataverse.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 04:13:43 2026 GMT\n  hsts: null\ndomains:\n- domain: dataverse.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dataverse/refs/heads/main/security/dataverse-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
---
