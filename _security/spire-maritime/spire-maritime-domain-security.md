---
description: ''
domains:
- caa: []
  caa_note: No CAA records returned at probe time.
  dmarc: true
  dmarc_note: v=DMARC1; p=none; rua=mailto:dmarc-reports@spire.com
  dmarc_policy: none
  dnssec: false
  domain: spire.com
  spf: true
  spf_note: v=spf1 with multiple includes (Google, Office365, SendGrid, Mandrill, HubSpot, Zendesk) and ~all.
hosts:
- cert_expires: Sep 14 00:11:44 2026 GMT
  host: spire.com
  hsts: false
  hsts_note: No Strict-Transport-Security header returned on the root document at probe time.
  https: true
  tls_version: TLSv1.3
- cert_expires: Jun 18 21:22:32 2027 GMT
  host: api.spire.com
  hsts: false
  hsts_note: GraphQL host; no HSTS header observed on probe (GraphQL requires POST + auth).
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 08:52:42 2026 GMT
  host: documentation.spire.com
  hsts: false
  hsts_note: 301-redirects to servicedocs-sm.kpler.com following the Kpler acquisition.
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spire Maritime Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spire Maritime, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Spire Maritime
provider_slug: spire-maritime
slug: spire-maritime-domain-security
source_filename: spire-maritime-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + GraphQL hosts\nhosts:\n- host: spire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 00:11:44 2026 GMT\n  hsts: false\n  hsts_note: No Strict-Transport-Security header returned on the root document at probe time.\n- host: api.spire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jun 18 21:22:32 2027 GMT\n  hsts: false\n  hsts_note: GraphQL host; no HSTS header observed on probe (GraphQL requires POST + auth).\n- host: documentation.spire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 08:52:42 2026 GMT\n  hsts: false\n  hsts_note: 301-redirects to servicedocs-sm.kpler.com following the Kpler acquisition.\ndomains:\n- domain: spire.com\n  dnssec: false\n  caa: []\n  caa_note: No CAA records returned at probe time.\n  spf: true\n  spf_note: v=spf1 with multiple includes (Google, Office365, SendGrid, Mandrill, HubSpot, Zendesk) and ~all.\n \
  \ dmarc: true\n  dmarc_policy: none\n  dmarc_note: v=DMARC1; p=none; rua=mailto:dmarc-reports@spire.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spire-maritime/refs/heads/main/security/spire-maritime-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Vessel Tracking
- AIS
- Maritime
- Satellite AIS
- Ship Tracking
- Real-Time Data
- Maritime Data
- Predicted ETA
- Port Events
- Location
- GraphQL
---
