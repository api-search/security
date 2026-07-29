---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dmarc_record: v=DMARC1; p=none; rua=mailto:ssc.dmarc.spc@canada.ca,mailto:dmarc@cyber.gc.ca; adkim=s; aspf=s
  dnssec: false
  domain: canada.ca
  note: Strict alignment (adkim=s, aspf=s) but the policy is still p=none, so no enforcement. Aggregate reports go to Shared Services Canada and to the Canadian Centre for Cyber Security.
  spf: true
  spf_record: v=spf1 include:emrs._spf.ssc-spc.gc.ca include:spf.protection.outlook.com include:slms._spf.ssc-spc.gc.ca -all
- caa: []
  dmarc: true
  dmarc_policy: none
  dmarc_record: v=DMARC1; p=none; sp=none; rua=mailto:dmarc@cyber.gc.ca
  dnssec: false
  domain: gc.ca
  note: The API host data.tc.gc.ca sits under this domain.
  spf: true
  spf_record: v=spf1 mx include:spf.protection.outlook.com -all
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_record: v=DMARC1; p=reject;rua=mailto:nrcan.gcc-notifications-notifications-ncg.rncan@canada.ca
  dnssec: false
  domain: geo.ca
  note: The only enforcing DMARC policy in the set — and it belongs to Natural Resources Canada's geospatial platform, not to Transport Canada.
  spf: true
  spf_record: v=spf1 -all
hosts:
- cert_expires: Oct 18 02:15:03 2026 GMT
  host: tc.canada.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  role: departmental website
  tls_version: TLSv1.2
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: open.canada.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  role: open data portal + CKAN Action API (Treasury Board Secretariat)
  tls_version: TLSv1.3
- cert_expires: Sep 25 04:00:00 2026 GMT
  cert_issuer: C=US, O=SSL Corporation, CN=Entrust OV TLS Issuing RSA CA 1
  cert_subject: C=CA, ST=Quebec, L=Gatineau, O=Shared Services Canada, CN=data.tc.gc.ca
  chain_complete: false
  finding: 'The server sends the leaf certificate only and does not send the Entrust intermediate. openssl s_client returns "verify error:num=20:unable to get local issuer certificate" and "Verify return code: 21 (unable to verify the first certificate)". Clients that happen to have the intermediate cached (macOS keychain, most browsers) connect fine; a clean client, a container, or a language runtime using only a root bundle will fail TLS verification against Transport Canada''s only first-party API host. Verified twice — Python ssl and openssl s_client both fail, curl on macOS succeeds.'
  host: data.tc.gc.ca
  hsts: true
  hsts_directives: includeSubDomains; preload
  hsts_max_age: 31536000
  https: true
  role: Vehicle Recalls Database API host
  tls_version: TLSv1.2
- cert_expires: Feb  2 23:59:59 2027 GMT
  cert_issuer: C=US, O=Amazon, CN=Amazon RSA 2048 M04
  chain_complete: true
  host: maps-cartes.services.geo.ca
  hsts: false
  https: true
  note: Verify return code 0 (ok). No Strict-Transport-Security header on the root (the root answers 301). Hosted on AWS, unlike the departmental estate.
  role: Canadian Airports ArcGIS REST + OGC WMS host (NRCan Federal Geospatial Platform)
  tls_version: TLSv1.2
- cert_expires: Oct 18 02:15:03 2026 GMT
  cert_issuer: C=US, O=Let's Encrypt, CN=YR1
  chain_complete: true
  host: opendatatc.tc.canada.ca
  hsts: false
  https: true
  note: No HSTS header observed. This host carries the CADORS, vehicle recall, Air Cargo Security and vessel register extracts — the de facto primary distribution channel for Transport Canada data.
  role: bulk CSV/XML distribution host
kind: domain-security
layout: security
method: probed
name: Transport Canada Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transport Canada, probed live across 5 host(s) and 3 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Transport Canada
provider_slug: transport-canada
slug: transport-canada-domain-security
source_filename: transport-canada-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nsource: >-\n  Live DNS/TLS/HTTP probes of every apis.yml host on 2026-07-28, run with\n  0-working/probe-domain-security.py and then extended by hand to cover the\n  geospatial and bulk-file hosts the script does not read out of apis.yml\n  (maps-cartes.services.geo.ca, opendatatc.tc.canada.ca) and to verify the\n  data.tc.gc.ca chain finding with openssl s_client.\nhosts:\n- host: tc.canada.ca\n  role: departmental website\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 18 02:15:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: open.canada.ca\n  role: open data portal + CKAN Action API (Treasury Board Secretariat)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data.tc.gc.ca\n  role: Vehicle Recalls Database API host\n  https: true\n  tls_version: TLSv1.2\n  cert_issuer: C=US, O=SSL Corporation, CN=Entrust OV TLS Issuing RSA CA 1\n\
  \  cert_subject: C=CA, ST=Quebec, L=Gatineau, O=Shared Services Canada, CN=data.tc.gc.ca\n  cert_expires: Sep 25 04:00:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_directives: includeSubDomains; preload\n  chain_complete: false\n  finding: >-\n    The server sends the leaf certificate only and does not send the Entrust\n    intermediate. openssl s_client returns \"verify error:num=20:unable to get\n    local issuer certificate\" and \"Verify return code: 21 (unable to verify the\n    first certificate)\". Clients that happen to have the intermediate cached\n    (macOS keychain, most browsers) connect fine; a clean client, a container,\n    or a language runtime using only a root bundle will fail TLS verification\n    against Transport Canada's only first-party API host. Verified twice —\n    Python ssl and openssl s_client both fail, curl on macOS succeeds.\n- host: maps-cartes.services.geo.ca\n  role: Canadian Airports ArcGIS REST + OGC WMS host (NRCan Federal Geospatial\
  \ Platform)\n  https: true\n  tls_version: TLSv1.2\n  cert_issuer: C=US, O=Amazon, CN=Amazon RSA 2048 M04\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  chain_complete: true\n  hsts: false\n  note: >-\n    Verify return code 0 (ok). No Strict-Transport-Security header on the root\n    (the root answers 301). Hosted on AWS, unlike the departmental estate.\n- host: opendatatc.tc.canada.ca\n  role: bulk CSV/XML distribution host\n  https: true\n  cert_issuer: C=US, O=Let's Encrypt, CN=YR1\n  cert_expires: Oct 18 02:15:03 2026 GMT\n  chain_complete: true\n  hsts: false\n  note: >-\n    No HSTS header observed. This host carries the CADORS, vehicle recall, Air\n    Cargo Security and vessel register extracts — the de facto primary\n    distribution channel for Transport Canada data.\ndomains:\n- domain: canada.ca\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:emrs._spf.ssc-spc.gc.ca include:spf.protection.outlook.com include:slms._spf.ssc-spc.gc.ca -all\n  dmarc: true\n\
  \  dmarc_policy: none\n  dmarc_record: v=DMARC1; p=none; rua=mailto:ssc.dmarc.spc@canada.ca,mailto:dmarc@cyber.gc.ca; adkim=s; aspf=s\n  note: >-\n    Strict alignment (adkim=s, aspf=s) but the policy is still p=none, so no\n    enforcement. Aggregate reports go to Shared Services Canada and to the\n    Canadian Centre for Cyber Security.\n- domain: gc.ca\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 mx include:spf.protection.outlook.com -all\n  dmarc: true\n  dmarc_policy: none\n  dmarc_record: v=DMARC1; p=none; sp=none; rua=mailto:dmarc@cyber.gc.ca\n  note: The API host data.tc.gc.ca sits under this domain.\n- domain: geo.ca\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 -all\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_record: v=DMARC1; p=reject;rua=mailto:nrcan.gcc-notifications-notifications-ncg.rncan@canada.ca\n  note: >-\n    The only enforcing DMARC policy in the set — and it belongs to Natural\n    Resources Canada's geospatial platform, not\
  \ to Transport Canada.\nsummary:\n  https_everywhere: true\n  tls13: 1 of 5 hosts (open.canada.ca)\n  hsts: 3 of 5 hosts\n  dnssec: 0 of 3 domains\n  caa: 0 of 3 domains\n  dmarc_enforcing: 1 of 3 domains (geo.ca, p=reject)\n  notable: >-\n    Two findings stand out. First, data.tc.gc.ca — the department's only\n    first-party API host — serves an incomplete certificate chain. Second, no\n    domain in the estate publishes CAA records or DNSSEC, and the two\n    Government of Canada apex domains carry non-enforcing DMARC (p=none).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transport-canada/refs/heads/main/security/transport-canada-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Travel
- Canada
- Aviation
- Regulator
- Government
- Airports
- Aircraft Registry
- Aviation Safety
- Drones
- Open Data
- Transportation
---
