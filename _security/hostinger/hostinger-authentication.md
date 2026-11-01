---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Hostinger Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hostinger secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hostinger
provider_slug: hostinger
scheme_count: 1
schemes:
- description: API Token authentication
  name: apiToken
  scheme: bearer
  sources:
  - openapi/hostinger-agency-hosting-cache-api-openapi.yml
  - openapi/hostinger-agency-hosting-cron-jobs-api-openapi.yml
  - openapi/hostinger-agency-hosting-databases-api-openapi.yml
  - openapi/hostinger-agency-hosting-datacenters-api-openapi.yml
  - openapi/hostinger-agency-hosting-domains-api-openapi.yml
  - openapi/hostinger-agency-hosting-files-api-openapi.yml
  - openapi/hostinger-agency-hosting-metrics-api-openapi.yml
  - openapi/hostinger-agency-hosting-orders-api-openapi.yml
  - openapi/hostinger-agency-hosting-php-api-openapi.yml
  - openapi/hostinger-agency-hosting-ssl-api-openapi.yml
  - openapi/hostinger-agency-hosting-website-setups-api-openapi.yml
  - openapi/hostinger-agency-hosting-websites-api-openapi.yml
  - openapi/hostinger-agency-hosting-wordpress-api-openapi.yml
  - openapi/hostinger-agent-readiness-checks-api-openapi.yml
  - openapi/hostinger-agent-readiness-scans-api-openapi.yml
  - openapi/hostinger-billing-catalog-api-openapi.yml
  - openapi/hostinger-billing-orders-api-openapi.yml
  - openapi/hostinger-billing-payment-methods-api-openapi.yml
  - openapi/hostinger-billing-subscriptions-api-openapi.yml
  - openapi/hostinger-dns-snapshot-api-openapi.yml
  - openapi/hostinger-dns-zone-api-openapi.yml
  - openapi/hostinger-domain-access-verifier-verifications-api-openapi.yml
  - openapi/hostinger-domains-availability-api-openapi.yml
  - openapi/hostinger-domains-forwarding-api-openapi.yml
  - openapi/hostinger-domains-move-api-openapi.yml
  - openapi/hostinger-domains-portfolio-api-openapi.yml
  - openapi/hostinger-domains-transfer-api-openapi.yml
  - openapi/hostinger-domains-whois-api-openapi.yml
  - openapi/hostinger-ecommerce-discounts-api-openapi.yml
  - openapi/hostinger-ecommerce-miscellaneous-api-openapi.yml
  - openapi/hostinger-ecommerce-orders-api-openapi.yml
  - openapi/hostinger-ecommerce-payments-api-openapi.yml
  - openapi/hostinger-ecommerce-product-variants-api-openapi.yml
  - openapi/hostinger-ecommerce-products-api-openapi.yml
  - openapi/hostinger-ecommerce-sales-channels-api-openapi.yml
  - openapi/hostinger-ecommerce-shipping-api-openapi.yml
  - openapi/hostinger-ecommerce-stores-api-openapi.yml
  - openapi/hostinger-horizons-websites-api-openapi.yml
  - openapi/hostinger-hosting-cache-api-openapi.yml
  - openapi/hostinger-hosting-cdn-api-openapi.yml
  - openapi/hostinger-hosting-cron-jobs-api-openapi.yml
  - openapi/hostinger-hosting-databases-api-openapi.yml
  - openapi/hostinger-hosting-datacenters-api-openapi.yml
  - openapi/hostinger-hosting-domains-api-openapi.yml
  - openapi/hostinger-hosting-files-api-openapi.yml
  - openapi/hostinger-hosting-git-api-openapi.yml
  - openapi/hostinger-hosting-headless-api-openapi.yml
  - openapi/hostinger-hosting-nodejs-api-openapi.yml
  - openapi/hostinger-hosting-orders-api-openapi.yml
  - openapi/hostinger-hosting-php-api-openapi.yml
  - openapi/hostinger-hosting-redirects-api-openapi.yml
  - openapi/hostinger-hosting-ssl-api-openapi.yml
  - openapi/hostinger-hosting-websites-api-openapi.yml
  - openapi/hostinger-mail-aliases-api-openapi.yml
  - openapi/hostinger-mail-api-tokens-api-openapi.yml
  - openapi/hostinger-mail-autoreplies-api-openapi.yml
  - openapi/hostinger-mail-catchalls-api-openapi.yml
  - openapi/hostinger-mail-forwarders-api-openapi.yml
  - openapi/hostinger-mail-logs-api-openapi.yml
  - openapi/hostinger-mail-mailboxes-api-openapi.yml
  - openapi/hostinger-mail-orders-api-openapi.yml
  - openapi/hostinger-mail-webhooks-api-openapi.yml
  - openapi/hostinger-reach-automations-api-openapi.yml
  - openapi/hostinger-reach-campaigns-api-openapi.yml
  - openapi/hostinger-reach-contact-fields-api-openapi.yml
  - openapi/hostinger-reach-contacts-api-openapi.yml
  - openapi/hostinger-reach-forms-api-openapi.yml
  - openapi/hostinger-reach-profiles-api-openapi.yml
  - openapi/hostinger-reach-segments-api-openapi.yml
  - openapi/hostinger-reach-tags-api-openapi.yml
  - openapi/hostinger-reach-templates-api-openapi.yml
  - openapi/hostinger-vps-actions-api-openapi.yml
  - openapi/hostinger-vps-backups-api-openapi.yml
  - openapi/hostinger-vps-data-centers-api-openapi.yml
  - openapi/hostinger-vps-docker-manager-api-openapi.yml
  - openapi/hostinger-vps-firewall-api-openapi.yml
  - openapi/hostinger-vps-malware-scanner-api-openapi.yml
  - openapi/hostinger-vps-os-templates-api-openapi.yml
  - openapi/hostinger-vps-post-install-scripts-api-openapi.yml
  - openapi/hostinger-vps-ptr-records-api-openapi.yml
  - openapi/hostinger-vps-public-keys-api-openapi.yml
  - openapi/hostinger-vps-recovery-api-openapi.yml
  - openapi/hostinger-vps-snapshots-api-openapi.yml
  - openapi/hostinger-vps-ssh-keys-api-openapi.yml
  - openapi/hostinger-vps-virtual-machine-api-openapi.yml
  - openapi/hostinger-wordpress-ai-content-api-openapi.yml
  - openapi/hostinger-wordpress-ai-tools-api-openapi.yml
  - openapi/hostinger-wordpress-installations-api-openapi.yml
  - openapi/hostinger-wordpress-litespeed-cache-api-openapi.yml
  - openapi/hostinger-wordpress-login-api-openapi.yml
  - openapi/hostinger-wordpress-maintenance-api-openapi.yml
  - openapi/hostinger-wordpress-object-cache-api-openapi.yml
  - openapi/hostinger-wordpress-plugins-api-openapi.yml
  - openapi/hostinger-wordpress-themes-api-openapi.yml
  type: http
slug: hostinger-authentication
source_filename: hostinger-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: derived\nsource: openapi/hostinger-agency-hosting-cache-api-openapi.yml, openapi/hostinger-agency-hosting-cron-jobs-api-openapi.yml,\n  openapi/hostinger-agency-hosting-databases-api-openapi.yml, openapi/hostinger-agency-hosting-datacenters-api-openapi.yml,\n  openapi/hostinger-agency-hosting-domains-api-openapi.yml, openapi/hostinger-agency-hosting-files-api-openapi.yml,\n  openapi/hostinger-agency-hosting-metrics-api-openapi.yml, openapi/hostinger-agency-hosting-orders-api-openapi.yml,\n  openapi/hostinger-agency-hosting-php-api-openapi.yml, openapi/hostinger-agency-hosting-ssl-api-openapi.yml,\n  openapi/hostinger-agency-hosting-website-setups-api-openapi.yml, openapi/hostinger-agency-hosting-websites-api-openapi.yml\n  ...\nsummary:\n  types:\n  - http\nschemes:\n- name: apiToken\n  type: http\n  scheme: bearer\n  description: API Token authentication\n  sources:\n  - openapi/hostinger-agency-hosting-cache-api-openapi.yml\n  - openapi/hostinger-agency-hosting-cron-jobs-api-openapi.yml\n\
  \  - openapi/hostinger-agency-hosting-databases-api-openapi.yml\n  - openapi/hostinger-agency-hosting-datacenters-api-openapi.yml\n  - openapi/hostinger-agency-hosting-domains-api-openapi.yml\n  - openapi/hostinger-agency-hosting-files-api-openapi.yml\n  - openapi/hostinger-agency-hosting-metrics-api-openapi.yml\n  - openapi/hostinger-agency-hosting-orders-api-openapi.yml\n  - openapi/hostinger-agency-hosting-php-api-openapi.yml\n  - openapi/hostinger-agency-hosting-ssl-api-openapi.yml\n  - openapi/hostinger-agency-hosting-website-setups-api-openapi.yml\n  - openapi/hostinger-agency-hosting-websites-api-openapi.yml\n  - openapi/hostinger-agency-hosting-wordpress-api-openapi.yml\n  - openapi/hostinger-agent-readiness-checks-api-openapi.yml\n  - openapi/hostinger-agent-readiness-scans-api-openapi.yml\n  - openapi/hostinger-billing-catalog-api-openapi.yml\n  - openapi/hostinger-billing-orders-api-openapi.yml\n  - openapi/hostinger-billing-payment-methods-api-openapi.yml\n  - openapi/hostinger-billing-subscriptions-api-openapi.yml\n\
  \  - openapi/hostinger-dns-snapshot-api-openapi.yml\n  - openapi/hostinger-dns-zone-api-openapi.yml\n  - openapi/hostinger-domain-access-verifier-verifications-api-openapi.yml\n  - openapi/hostinger-domains-availability-api-openapi.yml\n  - openapi/hostinger-domains-forwarding-api-openapi.yml\n  - openapi/hostinger-domains-move-api-openapi.yml\n  - openapi/hostinger-domains-portfolio-api-openapi.yml\n  - openapi/hostinger-domains-transfer-api-openapi.yml\n  - openapi/hostinger-domains-whois-api-openapi.yml\n  - openapi/hostinger-ecommerce-discounts-api-openapi.yml\n  - openapi/hostinger-ecommerce-miscellaneous-api-openapi.yml\n  - openapi/hostinger-ecommerce-orders-api-openapi.yml\n  - openapi/hostinger-ecommerce-payments-api-openapi.yml\n  - openapi/hostinger-ecommerce-product-variants-api-openapi.yml\n  - openapi/hostinger-ecommerce-products-api-openapi.yml\n  - openapi/hostinger-ecommerce-sales-channels-api-openapi.yml\n  - openapi/hostinger-ecommerce-shipping-api-openapi.yml\n  - openapi/hostinger-ecommerce-stores-api-openapi.yml\n\
  \  - openapi/hostinger-horizons-websites-api-openapi.yml\n  - openapi/hostinger-hosting-cache-api-openapi.yml\n  - openapi/hostinger-hosting-cdn-api-openapi.yml\n  - openapi/hostinger-hosting-cron-jobs-api-openapi.yml\n  - openapi/hostinger-hosting-databases-api-openapi.yml\n  - openapi/hostinger-hosting-datacenters-api-openapi.yml\n  - openapi/hostinger-hosting-domains-api-openapi.yml\n  - openapi/hostinger-hosting-files-api-openapi.yml\n  - openapi/hostinger-hosting-git-api-openapi.yml\n  - openapi/hostinger-hosting-headless-api-openapi.yml\n  - openapi/hostinger-hosting-nodejs-api-openapi.yml\n  - openapi/hostinger-hosting-orders-api-openapi.yml\n  - openapi/hostinger-hosting-php-api-openapi.yml\n  - openapi/hostinger-hosting-redirects-api-openapi.yml\n  - openapi/hostinger-hosting-ssl-api-openapi.yml\n  - openapi/hostinger-hosting-websites-api-openapi.yml\n  - openapi/hostinger-mail-aliases-api-openapi.yml\n  - openapi/hostinger-mail-api-tokens-api-openapi.yml\n  - openapi/hostinger-mail-autoreplies-api-openapi.yml\n\
  \  - openapi/hostinger-mail-catchalls-api-openapi.yml\n  - openapi/hostinger-mail-forwarders-api-openapi.yml\n  - openapi/hostinger-mail-logs-api-openapi.yml\n  - openapi/hostinger-mail-mailboxes-api-openapi.yml\n  - openapi/hostinger-mail-orders-api-openapi.yml\n  - openapi/hostinger-mail-webhooks-api-openapi.yml\n  - openapi/hostinger-reach-automations-api-openapi.yml\n  - openapi/hostinger-reach-campaigns-api-openapi.yml\n  - openapi/hostinger-reach-contact-fields-api-openapi.yml\n  - openapi/hostinger-reach-contacts-api-openapi.yml\n  - openapi/hostinger-reach-forms-api-openapi.yml\n  - openapi/hostinger-reach-profiles-api-openapi.yml\n  - openapi/hostinger-reach-segments-api-openapi.yml\n  - openapi/hostinger-reach-tags-api-openapi.yml\n  - openapi/hostinger-reach-templates-api-openapi.yml\n  - openapi/hostinger-vps-actions-api-openapi.yml\n  - openapi/hostinger-vps-backups-api-openapi.yml\n  - openapi/hostinger-vps-data-centers-api-openapi.yml\n  - openapi/hostinger-vps-docker-manager-api-openapi.yml\n\
  \  - openapi/hostinger-vps-firewall-api-openapi.yml\n  - openapi/hostinger-vps-malware-scanner-api-openapi.yml\n  - openapi/hostinger-vps-os-templates-api-openapi.yml\n  - openapi/hostinger-vps-post-install-scripts-api-openapi.yml\n  - openapi/hostinger-vps-ptr-records-api-openapi.yml\n  - openapi/hostinger-vps-public-keys-api-openapi.yml\n  - openapi/hostinger-vps-recovery-api-openapi.yml\n  - openapi/hostinger-vps-snapshots-api-openapi.yml\n  - openapi/hostinger-vps-ssh-keys-api-openapi.yml\n  - openapi/hostinger-vps-virtual-machine-api-openapi.yml\n  - openapi/hostinger-wordpress-ai-content-api-openapi.yml\n  - openapi/hostinger-wordpress-ai-tools-api-openapi.yml\n  - openapi/hostinger-wordpress-installations-api-openapi.yml\n  - openapi/hostinger-wordpress-litespeed-cache-api-openapi.yml\n  - openapi/hostinger-wordpress-login-api-openapi.yml\n  - openapi/hostinger-wordpress-maintenance-api-openapi.yml\n  - openapi/hostinger-wordpress-object-cache-api-openapi.yml\n  - openapi/hostinger-wordpress-plugins-api-openapi.yml\n\
  \  - openapi/hostinger-wordpress-themes-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/hostinger/authentication/hostinger-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Hosting
- Cloud
- Domains
- API
---
