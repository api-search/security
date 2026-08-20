---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_record: v=DMARC1; p=reject; aspf=s; rua=mailto:rzrknxeawk@rua.powerdmarc.com; fo=0:1:d:s; t=n;
  dnssec: false
  domain: prudentialplc.com
  note: The only domain in the estate at p=reject, with strict SPF alignment (aspf=s). The _dmarc record is a CNAME into hosteddmarc.dmarc-dns.com, confirming a managed DMARC service.
  spf: true
  spf_record: v=spf1 include:7fg5yhj2mj.powerspf.com -all
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: prudential.com.hk
  spf: true
  spf_record: v=spf1 include:1smpil468z.powerspf.com -all
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: prudential.com.sg
  spf: true
  spf_record: v=spf1 include:e91ggo5akw.powerspf.com -all
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  dnssec_ds: 41055 13 2 B3D906BCC31C0CB11609160641E76C9D85815087DDC109B8AE3F7EEC54E2AF74
  domain: prudential.co.id
  note: The only DNSSEC-signed domain found in the estate (algorithm 13, ECDSA P-256 SHA-256).
  spf: true
  spf_record: v=spf1 include:epedd15chq.powerspf.com -all
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: prudential.com.vn
  spf: true
  spf_record: v=spf1 include:gru39w8qi1.powerspf.com -all
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: prulifeuk.com.ph
  note: Adds aspf=s (strict SPF alignment) to the group's standard quarantine policy.
  spf: true
  spf_record: v=spf1 include:8wuhbgo5wi.powerspf.com -all
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: prubsn.com.my
  spf: true
  spf_record: v=spf1 include:bzxv93thzz.powerspf.com -all
hosts:
- cert_expires: Oct  9 06:45:13 2026 GMT
  host: www.prudentialplc.com
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31557600
  hsts_preload: false
  https: true
  role: group corporate site
  tls_version: TLSv1.3
- cert_expires: Sep 24 04:28:38 2026 GMT
  host: www.prudential.com.hk
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31557600
  hsts_preload: false
  https: true
  role: Prudential Hong Kong Limited
  tls_version: TLSv1.3
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: www.prudential.com.sg
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  note: The only host in the estate with includeSubDomains and preload - the strongest HSTS posture in the group.
  role: Prudential Assurance Company Singapore
  tls_version: TLSv1.3
- cert_expires: Oct  9 06:45:13 2026 GMT
  host: www.prudential.co.id
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31557600
  hsts_preload: false
  https: true
  role: PT Prudential Life Assurance
  tls_version: TLSv1.3
- cert_expires: Oct  8 16:33:45 2026 GMT
  host: www.prudential.com.vn
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31557600
  hsts_preload: false
  https: true
  role: Prudential Vietnam Assurance
  tls_version: TLSv1.3
- cert_expires: Oct  8 16:33:45 2026 GMT
  host: www.prulifeuk.com.ph
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31557600
  hsts_preload: false
  https: true
  role: Pru Life UK
  tls_version: TLSv1.3
- cert_expires: Oct  8 16:33:45 2026 GMT
  host: www.prubsn.com.my
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31557600
  hsts_preload: false
  https: true
  role: Prudential BSN Takaful Berhad
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prudential Plc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prudential plc, probed live across 7 host(s) and 7 registrable domain(s). 7 host(s) serve HTTPS (up to TLSv1.3); 7 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Prudential plc
provider_slug: prudential-plc
slug: prudential-plc-domain-security
source_filename: prudential-plc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: >-\n  live DNS/TLS/HTTP probes 2026-07-25 of the apis.yml host plus every resolvable\n  Prudential plc market operating-company host (extends the mechanical\n  0-working/probe-domain-security.py run, which covers only the apis.yml hosts)\nnote: >-\n  Prudential plc exposes no API host, so this profile covers the corporate site\n  and the market consumer sites instead. The result is the most positive\n  technical finding in this record: the group runs a visibly CENTRALISED email\n  and transport security posture across eleven jurisdictions - TLS 1.3\n  everywhere, HSTS everywhere, and one shared PowerDMARC/PowerSPF tenant with a\n  common aggregate-report mailbox on every domain. Absence of CAA and (mostly) of\n  DNSSEC is recorded as observed fact, not judgement.\nhosts:\n- host: www.prudentialplc.com\n  role: group corporate site\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 06:45:13 2026 GMT\n  hsts: true\n\
  \  hsts_max_age: 31557600\n  hsts_include_subdomains: false\n  hsts_preload: false\n- host: www.prudential.com.hk\n  role: Prudential Hong Kong Limited\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 04:28:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n  hsts_include_subdomains: false\n  hsts_preload: false\n- host: www.prudential.com.sg\n  role: Prudential Assurance Company Singapore\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: The only host in the estate with includeSubDomains and preload - the strongest HSTS posture in the group.\n- host: www.prudential.co.id\n  role: PT Prudential Life Assurance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 06:45:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n  hsts_include_subdomains: false\n  hsts_preload: false\n- host: www.prudential.com.vn\n  role: Prudential Vietnam\
  \ Assurance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 16:33:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n  hsts_include_subdomains: false\n  hsts_preload: false\n- host: www.prulifeuk.com.ph\n  role: Pru Life UK\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 16:33:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n  hsts_include_subdomains: false\n  hsts_preload: false\n- host: www.prubsn.com.my\n  role: Prudential BSN Takaful Berhad\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 16:33:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n  hsts_include_subdomains: false\n  hsts_preload: false\ndomains:\n- domain: prudentialplc.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:7fg5yhj2mj.powerspf.com -all\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_record: 'v=DMARC1; p=reject; aspf=s; rua=mailto:rzrknxeawk@rua.powerdmarc.com; fo=0:1:d:s; t=n;'\n  note: >-\n    The only domain in the estate at p=reject,\
  \ with strict SPF alignment\n    (aspf=s). The _dmarc record is a CNAME into hosteddmarc.dmarc-dns.com,\n    confirming a managed DMARC service.\n- domain: prudential.com.hk\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:1smpil468z.powerspf.com -all\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: prudential.com.sg\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:e91ggo5akw.powerspf.com -all\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: prudential.co.id\n  dnssec: true\n  dnssec_ds: 41055 13 2 B3D906BCC31C0CB11609160641E76C9D85815087DDC109B8AE3F7EEC54E2AF74\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:epedd15chq.powerspf.com -all\n  dmarc: true\n  dmarc_policy: quarantine\n  note: The only DNSSEC-signed domain found in the estate (algorithm 13, ECDSA P-256 SHA-256).\n- domain: prudential.com.vn\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:gru39w8qi1.powerspf.com -all\n  dmarc: true\n  dmarc_policy:\
  \ quarantine\n- domain: prulifeuk.com.ph\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:8wuhbgo5wi.powerspf.com -all\n  dmarc: true\n  dmarc_policy: quarantine\n  note: Adds aspf=s (strict SPF alignment) to the group's standard quarantine policy.\n- domain: prubsn.com.my\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:bzxv93thzz.powerspf.com -all\n  dmarc: true\n  dmarc_policy: quarantine\ngroup_posture:\n  centralised_email_security: true\n  evidence: >-\n    All seven domains publish an SPF record of the identical shape\n    \"v=spf1 include:<tenant-hash>.powerspf.com -all\" with a hard fail, and all\n    seven publish a DMARC record whose aggregate-report address is the SAME\n    mailbox, rzrknxeawk@rua.powerdmarc.com, with several also adding a local\n    market rua. That is one PowerDMARC tenant administered centrally for the\n    whole group rather than seven independently managed estates.\n  tls: TLS 1.3 on every host probed; no host\
  \ fell back below TLS 1.2.\n  hsts: HSTS present on every host; six of seven use max-age 31557600 (one year in seconds, Adobe Experience Manager default), Singapore alone uses 31536000 with includeSubDomains and preload.\n  dnssec: 1 of 7 domains signed (prudential.co.id).\n  caa: 0 of 7 domains publish a CAA record - certificate issuance is unconstrained at DNS level across the entire estate.\n  gap: >-\n    The clearest actionable gap. Adding CAA records and lifting the market\n    domains from p=quarantine to p=reject would cost nothing and would match the\n    discipline already demonstrated by the shared SPF/DMARC tenancy.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prudential-plc/refs/heads/main/security/prudential-plc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Insurance
- United Kingdom
- Life Insurance
- Health Insurance
- Carrier
- Asset Management
- Pensions
- Takaful
- Bancassurance
- Asia
- Africa
- Hong Kong
- Singapore
- Malaysia
- Indonesia
- Vietnam
- Philippines
- Eastspring
- Responsible AI
- llms-txt
---
