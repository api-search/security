---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: iliadbio.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: iliadbiotech.com
  spf: true
hosts:
- cert_expires: Sep 23 10:35:22 2026 GMT
  host: iliadbio.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan  9 18:18:09 2027 GMT
  cert_issuer: GoDaddy TLS Intermediate CA DV - R1v1
  host: iliadbiotech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iliad Biotechnologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ILiAD Biotechnologies, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: ILiAD Biotechnologies
provider_slug: iliad-biotechnologies
slug: iliad-biotechnologies-domain-security
source_filename: iliad-biotechnologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts (2026-08-22)\nnote: >-\n  ILiAD runs two domains — iliadbio.com serves the public website, iliadbiotech.com carries\n  corporate mail (info@iliadbiotech.com) and 301s web traffic to iliadbio.com. Both were probed.\n  Neither publishes CAA records and neither is DNSSEC-signed; iliadbio.com sends no HSTS header\n  and has no SPF record, while iliadbiotech.com publishes SPF (Barracuda + Microsoft 365) and a\n  DMARC policy of quarantine. Absence of a record is recorded as measured, not inferred.\nhosts:\n- host: iliadbio.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 23 10:35:22 2026 GMT\n  hsts: false\n- host: iliadbiotech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 18:18:09 2027 GMT\n  cert_issuer: GoDaddy TLS Intermediate CA DV - R1v1\n  hsts: false\ndomains:\n- domain: iliadbio.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy:\
  \ none\n- domain: iliadbiotech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iliad-biotechnologies/refs/heads/main/security/iliad-biotechnologies-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Biotechnology
- Vaccines
- Life Sciences
- Pharmaceuticals
- Health
- Immunology
- Infectious Disease
- Clinical Trials
---
