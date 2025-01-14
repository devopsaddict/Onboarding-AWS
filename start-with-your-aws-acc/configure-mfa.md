# configure MFA in IAM
### For free increased security AWS recommends to setup Multi-Factor Authentication
## MFA types
#### Contents
  - passkeys and security keys
  - virtual auth applications
  - harware totp tokens

#### To enable a passkey or security key for your root user (console)
  - Open the [AWS Management Console](https://console.aws.amazon.com/) and signin using root creds
  - On the right side of the navigation bar, choose your account name, and then choose **Security credentials**
    
      ![AWS Security Credentials!](https://docs.aws.amazon.com/images/IAM/latest/UserGuide/images/security-credentials-root.shared.console.png "AWS Security Credentials")

  - On your root user **My security credentials** page, under **Multi-factor authentication (MFA)**, choose **Assign MFA device**
  - On the **MFA device name** page, enter a **Device name**, choose **Passkey or Security Key**, and then choose **Next**.
  - On **Set up device**, set up your passkey. Create a passkey with biometric data like your face or fingerprint, with a device pin, or by inserting the FIDO security key into your computer's USB port and tapping it.
  - Follow the instructions on your browser to choose a passkey provider or where you want to store your passkey to use across your devices
  - Choose **Continue**

You have now registered your passkey for use with AWS. The next time you use your root user credentials to sign in, you must authenticate with your passkey to complete the sign-in process.

