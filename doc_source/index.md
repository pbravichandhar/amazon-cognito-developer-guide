# Amazon Cognito Developer Guide

-----
*****Copyright &copy; Amazon Web Services, Inc. and/or its affiliates. All rights reserved.*****

-----
Amazon's trademarks and trade dress may not be used in 
     connection with any product or service that is not Amazon's, 
     in any manner that is likely to cause confusion among customers, 
     or in any manner that disparages or discredits Amazon. All other 
     trademarks not owned by Amazon are the property of their respective
     owners, who may or may not be affiliated with, connected to, or 
     sponsored by Amazon.

-----
## Contents
+ [What is Amazon Cognito?](what-is-amazon-cognito.md)
   + [Using the Amazon Cognito console](cognito-console.md)
+ [Getting started with Amazon Cognito](cognito-getting-started.md)
+ [Common Amazon Cognito scenarios](cognito-scenarios.md)
+ [Amazon Cognito tutorials](tutorials.md)
   + [Tutorial: Creating a user pool](tutorial-create-user-pool.md)
   + [Tutorial: Creating an identity pool](tutorial-create-identity-pool.md)
   + [Tutorial: Cleaning up your AWS resources](tutorial-cleanup-tutorial.md)
+ [Integrating Amazon Cognito with web and mobile apps](cognito-integrate-apps.md)
+ [Multi-tenant application best practices](multi-tenant-application-best-practices.md)
   + [User pool-based multi-tenancy](bp_user-pool-based-multi-tenancy.md)
   + [Application client-based multi-tenancy](application-client-based-multi-tenancy.md)
   + [Group-based multi-tenancy](group-based-multi-tenancy.md)
   + [Custom attribute-based multi-tenancy](custom-attribute-based-multi-tenancy.md)
   + [Multi-tenancy security recommendations](multi-tenancy-security-recommendations.md)
+ [Amazon Cognito user pools](cognito-user-identity-pools.md)
   + [Getting started with user pools](getting-started-with-cognito-user-pools.md)
      + [Prerequisite: Sign up for an AWS account](aws-cognito-sign-up-aws-account.md)
      + [Step 1. Create a user pool](cognito-user-pool-as-user-directory.md)
      + [Step 2. Add an app to enable the hosted web UI](cognito-user-pools-configuring-app-integration.md)
      + [Step 3. Add social sign-in to a user pool (optional)](cognito-user-pools-configuring-federation-with-social-idp.md)
      + [Step 4. Add sign-in with a SAML identity provider to a user pool (optional)](cognito-user-pools-configuring-federation-with-saml-2-0-idp.md)
      + [Next steps](user-pool-next-steps.md)
   + [Using the Amazon Cognito hosted UI for sign-up and sign-in](cognito-user-pools-app-integration.md)
      + [Configuring a user pool app client](cognito-user-pools-app-idp-settings.md)
      + [Configuring a user pool domain](cognito-user-pools-assign-domain.md)
         + [Using the Amazon Cognito domain for the hosted UI](cognito-user-pools-assign-domain-prefix.md)
         + [Using your own domain for the hosted UI](cognito-user-pools-add-custom-domain.md)
      + [Customizing the built-in sign-in and sign-up webpages](cognito-user-pools-app-ui-customization.md)
      + [Defining resource servers for your user pool](cognito-user-pools-define-resource-servers.md)
   + [Adding user pool sign-in through a third party](cognito-user-pools-identity-federation.md)
      + [Adding social identity providers to a user pool](cognito-user-pools-social-idp.md)
      + [Adding SAML identity providers to a user pool](cognito-user-pools-saml-idp.md)
         + [SAML user pool IdP authentication flow](cognito-user-pools-saml-idp-authentication.md)
         + [Choosing SAML identity provider names](cognito-user-pools-managing-saml-idp-naming.md)
         + [Creating and managing a SAML identity provider for a user pool (AWS Management Console)](cognito-user-pools-managing-saml-idp-console.md)
         + [Creating and managing a SAML identity provider for a user pool (AWS CLI and AWS API)](cognito-user-pools-managing-saml-idp-cli-api.md)
         + [Integrating third-party SAML identity providers with Amazon Cognito user pools](cognito-user-pools-integrating-3rd-party-saml-providers.md)
      + [Adding OIDC identity providers to a user pool](cognito-user-pools-oidc-idp.md)
         + [OIDC user pool IdP authentication flow](cognito-user-pools-oidc-flow.md)
      + [Specifying identity provider attribute mappings for your user pool](cognito-user-pools-specifying-attribute-mapping.md)
   + [Customizing user pool workflows with Lambda triggers](cognito-user-identity-pools-working-with-aws-lambda-triggers.md)
      + [Pre sign-up Lambda trigger](user-pool-lambda-pre-sign-up.md)
      + [Post confirmation Lambda trigger](user-pool-lambda-post-confirmation.md)
      + [Pre authentication Lambda trigger](user-pool-lambda-pre-authentication.md)
      + [Post authentication Lambda trigger](user-pool-lambda-post-authentication.md)
      + [Custom authentication challenge Lambda triggers](user-pool-lambda-challenge.md)
         + [Define Auth challenge Lambda trigger](user-pool-lambda-define-auth-challenge.md)
         + [Create Auth challenge Lambda trigger](user-pool-lambda-create-auth-challenge.md)
         + [Verify Auth challenge response Lambda trigger](user-pool-lambda-verify-auth-challenge-response.md)
      + [Pre token generation Lambda trigger](user-pool-lambda-pre-token-generation.md)
      + [Migrate user Lambda trigger](user-pool-lambda-migrate-user.md)
      + [Custom message Lambda trigger](user-pool-lambda-custom-message.md)
      + [Custom sender Lambda triggers](user-pool-lambda-custom-sender-triggers.md)
         + [Custom email Lambda trigger](user-pool-lambda-custom-email-sender.md)
         + [Custom SMS sender Lambda trigger](user-pool-lambda-custom-sms-sender.md)
   + [Using Amazon Pinpoint analytics with Amazon Cognito user pools](cognito-user-pools-pinpoint-integration.md)
   + [Managing users in your user pool](managing-users.md)
      + [Signing up and confirming user accounts](signing-up-users-in-your-app.md)
      + [Creating user accounts as administrator](how-to-create-user-accounts.md)
      + [Adding groups to a user pool](cognito-user-pools-user-groups.md)
      + [Managing and searching for user accounts](how-to-manage-user-accounts.md)
      + [Recovering user accounts](how-to-recover-a-user-account.md)
      + [Importing users into a user pool](cognito-user-pools-import-users.md)
         + [Importing users into user pools with a user migration Lambda trigger](cognito-user-pools-import-using-lambda.md)
         + [Importing users into user pools from a CSV file](cognito-user-pools-using-import-tool.md)
            + [Creating the CloudWatch Logs IAM role (AWS CLI, API)](cognito-user-pools-using-import-tool-cli-cloudwatch-iam-role.md)
            + [Creating the user import .csv file](cognito-user-pools-using-import-tool-csv-header.md)
            + [Creating and running the Amazon Cognito user pool import job](cognito-user-pools-creating-import-job.md)
            + [Viewing the user pool import results in the CloudWatch console](cognito-user-pools-using-import-tool-cloudwatch.md)
            + [Requiring imported users to reset their passwords](cognito-user-pools-using-import-tool-password-reset.md)
   + [Email settings for Amazon Cognito user pools](user-pool-email.md)
   + [SMS message settings for Amazon Cognito user pools](user-pool-sms-settings.md)
   + [Using tokens with user pools](amazon-cognito-user-pools-using-tokens-with-identity-providers.md)
      + [Using the ID token](amazon-cognito-user-pools-using-the-id-token.md)
      + [Using the access token](amazon-cognito-user-pools-using-the-access-token.md)
      + [Using the refresh token](amazon-cognito-user-pools-using-the-refresh-token.md)
      + [Revoking tokens](token-revocation.md)
      + [Verifying a JSON web token](amazon-cognito-user-pools-using-tokens-verifying-a-jwt.md)
   + [Accessing resources after a successful user pool authentication](accessing-resources.md)
      + [Accessing server-side resources after sign-in](scenario-backend.md)
      + [Accessing resources with API Gateway and Lambda after sign-in](user-pool-accessing-resources-api-gateway-and-lambda.md)
      + [Accessing AWS services using an identity pool after sign-in](amazon-cognito-integrating-user-pools-with-identity-pools.md)
   + [User pools reference (AWS Management Console)](cognito-user-pools-getting-started-step-through-settings.md)
      + [Adding a user pool name](user-pool-settings-name.md)
      + [Importing and creating users and groups](user-pool-settings-users-and-groups.md)
      + [User pool attributes](user-pool-settings-attributes.md)
      + [Adding user pool password requirements](user-pool-settings-policies.md)
      + [Configuring an admin create user policy](user-pool-settings-admin-create-user-policy.md)
      + [Configuring email or phone verification](user-pool-settings-email-phone-verification.md)
      + [Configuring SMS and email verification messages and user invitation messages](cognito-user-pool-settings-message-customizations.md)
         + [Message templates](cognito-user-pool-settings-message-templates.md)
         + [Customizing the SMS message](cognito-user-pool-settings-SMS-message-customization.md)
         + [Customizing email verification messages](cognito-user-pool-settings-email-verification-message-customization.md)
         + [Customizing user invitation messages](cognito-user-pool-settings-user-invitation-message-customization.md)
         + [Customizing your email address](cognito-user-pool-settings-email-address-customization.md)
         + [Authorizing Amazon Cognito to send Amazon SES email on your behalf (from a custom FROM email address)](cognito-user-pool-settings-ses-authorization-to-send-email.md)
      + [Adding cost allocation tags to your user pool](cognito-user-pools-cost-allocation-tagging.md)
      + [Specifying user pool device tracking settings](amazon-cognito-user-pools-device-tracking.md)
      + [Configuring a user pool app client](user-pool-settings-client-apps.md)
      + [Configuring user pool Lambda triggers](user-pool-settings-triggers.md)
      + [Reviewing your user pool creation settings](review.md)
      + [Configuring user pool analytics](user-pool-settings-analytics.md)
      + [Configuring app client settings](cognito-user-pools-app-settings.md)
      + [Adding a domain name for your user pool](cognito-user-pools-domain.md)
      + [Customizing the built-in app UI to sign up and sign in users](cognito-user-pools-ux.md)
      + [Adding resource servers for your user pool](cognito-user-pools-resource-servers.md)
      + [Configuring identity providers for your user pool](cognito-user-pools-identity-provider.md)
      + [Configuring attribute mapping for your user pool](cognito-user-pools-attribute-mapping.md)
   + [Managing error responses](cognito-user-pool-managing-errors.md)
+ [Amazon Cognito identity pools (federated Identities)](cognito-identity.md)
   + [Getting started with Amazon Cognito identity pools (federated identities)](getting-started-with-identity-pools.md)
   + [Using identity pools (federated identities)](identity-pools.md)
      + [Managing datasets](managing-datasets-in-the-amazon-cognito-console.md)
      + [Bulk publish data](bulk-publish-data.md)
      + [Enable push synchronization](enable-push-synchronization.md)
      + [Set up Amazon Cognito Streams](set-up-cognito-streams.md)
      + [Set up Amazon Cognito Events](set-up-cognito-events.md)
   + [Identity pools concepts (federated identities)](concepts.md)
      + [Identity pools (federated identities) authentication flow](authentication-flow.md)
      + [IAM roles](iam-roles.md)
      + [Role trust and permissions](role-trust-and-permissions.md)
   + [Using attributes for access control as a form of attribute-based access control](attributes-for-access-control.md)
      + [Using attributes for access control with Amazon Cognito identity pools](using-afac-with-cognito-identity-pools.md)
      + [Using attributes for access control policy example](using-attributes-for-access-control-policy-example.md)
      + [Disable attributes for access control (console)](disable-afac.md)
      + [Default provider mappings](provider-mappings.md)
   + [Role-based access control](role-based-access-control.md)
   + [Getting credentials](getting-credentials.md)
   + [Accessing AWS services](accessing-aws-services.md)
   + [Identity pools (federated identities) external identity providers](external-identity-providers.md)
      + [Facebook (identity pools)](facebook.md)
      + [Login with Amazon (identity pools)](amazon.md)
      + [Google (identity pools)](google.md)
      + [Sign in with Apple (identity pools)](apple.md)
      + [Open ID Connect providers (identity pools)](open-id.md)
      + [SAML identity providers (identity pools)](saml-identity-provider.md)
   + [Developer authenticated identities (identity pools)](developer-authenticated-identities.md)
   + [Switching unauthenticated users to authenticated users (identity pools)](switching-identities.md)
+ [Amazon Cognito Sync](cognito-sync.md)
   + [Getting started with Amazon Cognito Sync](getting-started-with-cognito-sync.md)
   + [Synchronizing data](synchronizing-data.md)
   + [Handling callbacks](handling-callbacks.md)
   + [Push sync](push-sync.md)
   + [Amazon Cognito Streams](cognito-streams.md)
   + [Amazon Cognito Events](cognito-events.md)
+ [Security in Amazon Cognito](security.md)
   + [Data protection in Amazon Cognito](data-protection.md)
   + [Identity and access management for Amazon Cognito](security-iam.md)
      + [How Amazon Cognito works with IAM](security_iam_service-with-iam.md)
      + [Identity-based policy examples for Amazon Cognito](security_iam_id-based-policy-examples.md)
      + [Troubleshooting Amazon Cognito identity and access](security_iam_troubleshoot.md)
      + [Using service-linked roles for Amazon Cognito](using-service-linked-roles.md)
      + [Authentication with a user pool](authentication.md)
         + [User pool authentication flow](amazon-cognito-user-pools-authentication-flow.md)
   + [Logging and monitoring in Amazon Cognito](monitoring.md)
      + [Tracking quotas and usage in CloudWatch and Service Quotas](tracking-quotas-and-usage-in-cloud-watch-and-service-quotas.md)
      + [Metrics for Amazon Cognito user pools](metrics-for-cognito-user-pools.md)
      + [Dimensions for Amazon Cognito user pools](dimensions-for-cognito-user-pools.md)
      + [Use the Service Quotas console to track metrics](use-the-service-quota-console-to-track-metrics.md)
      + [Use the CloudWatch console to track metrics](use-the-cloud-watch-console-to-track-metrics.md)
      + [Create a CloudWatch alarm for a quota](create-a-cloud-watch-alarm.md)
      + [Logging Amazon Cognito API calls with AWS CloudTrail](logging-using-cloudtrail.md)
      + [Analyzing Amazon Cognito CloudTrail events with Amazon CloudWatch Logs Insights](analyzingcteventscwinsight.md)
   + [Compliance validation for Amazon Cognito](compliance-validation.md)
   + [Resilience in Amazon Cognito](disaster-recovery-resiliency.md)
      + [Regional data considerations](security-cognito-regional-data-considerations.md)
   + [Infrastructure security in Amazon Cognito](infrastructure-security.md)
   + [Configuration and vulnerability analysis in Amazon Cognito user pools](vulnerability-analysis-and-management.md)
   + [Security best practices for Amazon Cognito user pools](managing-security.md)
      + [Adding multi-factor authentication (MFA) to a user pool](user-pool-settings-mfa.md)
         + [SMS text message MFA](user-pool-settings-mfa-sms-text-message.md)
         + [TOTP software token MFA](user-pool-settings-mfa-totp.md)
      + [Adding advanced security to a user pool](cognito-user-pool-settings-advanced-security.md)
         + [Checking for compromised credentials](cognito-user-pool-settings-compromised-credentials.md)
         + [Using adaptive authentication](cognito-user-pool-settings-adaptive-authentication.md)
         + [Viewing advanced security metrics](user-pool-settings-viewing-advanced-security-metrics.md)
         + [Enabling user pool advanced security from your app](user-pool-settings-viewing-advanced-security-app.md)
   + [AWS managed policies for Amazon Cognito](security-iam-awsmanpol.md)
+ [Tagging Amazon Cognito resources](tagging.md)
+ [Quotas in Amazon Cognito](limits.md)
+ [Amazon Cognito API references](cognito-reference.md)
   + [Amazon Cognito user pools API reference](cognito-userpools-api-reference.md)
   + [Amazon Cognito user pools Auth API reference](cognito-userpools-server-contract-reference.md)
      + [AUTHORIZATION endpoint](authorization-endpoint.md)
      + [TOKEN endpoint](token-endpoint.md)
      + [USERINFO endpoint](userinfo-endpoint.md)
      + [LOGIN endpoint](login-endpoint.md)
      + [LOGOUT endpoint](logout-endpoint.md)
      + [REVOCATION endpoint](revocation-endpoint.md)
   + [Amazon Cognito identity pools (federated identities) API reference](cognito-federatedidentities-api-reference.md)
   + [Amazon Cognito sync API reference](cognito-sync-api-reference.md)
+ [Document history for Amazon Cognito](cognito-document-history.md)