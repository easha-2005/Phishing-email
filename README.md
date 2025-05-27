# Phishing-email
.

🛡️ Phishing Email Analysis Report
📌 Subject: "Refund Pending – IRCTC"
🖼️ Overview
This email is a simulated phishing attempt, appearing to come from IRCTC Helpdesk and offering a refund of ₹4,240 due to an alleged overcharge on an IRCTC transaction. The user is urged to scan a QR code and verify their mobile number to receive the refund.

🚩 Identified Red Flags
Suspicious Sender Email Address:

irtcc-helpdesk@securesupportcloud[.]com

Red Flag: The domain name is not related to IRCTC (Indian Railway Catering and Tourism Corporation). Legitimate emails from IRCTC would use @irctc.co.in.

Urgency/Time Limit:

Phrases like "This link will expire in 2 business days" are used to pressure the user into acting quickly.

Red Flag: Creating a sense of urgency is a common tactic in phishing to prevent careful consideration.

Unexpected Refund Claim:

The user is told of a refund without having initiated any complaint.

Red Flag: This is a classic phishing strategy — "free money" to lure users.

Use of QR Code:

QR codes are used to obscure the final destination URL.

Red Flag: Scanning the QR code might lead to credential harvesting or a malicious site.

Generic Language:

No personal identification, transaction ID, or booking reference is included.

Red Flag: Legitimate refund emails usually contain specific details related to the user’s account or transaction.

Email Layout and Branding:

IRCTC logo used, but poor formatting and layout suggest it's fake.

Red Flag: Visual identity may be spoofed but inconsistencies give it away.

📧 Simulated Email Header
text
Copy
Edit
Return-Path: <irtcc-helpdesk@securesupportcloud.com>
Received: from unknown (unknown [10.0.0.1])
  by mail.mybusiness.com with ESMTP id A1B2C3D4
  for <john.jdoe@mybusiness.com>; Mon, 27 May 2025 18:42:10 +0530
Received-SPF: Fail (mybusiness.com: domain of irtcc-helpdesk@securesupportcloud.com does not designate permitted sender hosts)
From: IRCTC Helpdesk <irtcc-helpdesk@securesupportcloud.com>
To: john.jdoe@mybusiness.com
Subject: Refund Pending
Date: Mon, 27 May 2025 18:42:10 +0530
Message-ID: <202505271842.A1B2C3D4@securesupportcloud.com>
MIME-Version: 1.0
Content-Type: text/html; charset="UTF-8"
🛠️ Tools Used for Header Analysis
MxToolbox (https://mxtoolbox.com/):

To check SPF, DKIM, and DMARC records.

Result here shows SPF fail (email sent from an unauthorized IP).

Google Admin Toolbox Messageheader (https://toolbox.googleapps.com/apps/messageheader/):

For parsing and visualizing email headers.

VirusTotal (https://www.virustotal.com/):

To scan URLs or domains extracted from QR codes.

QR Code Decoders:

e.g., zxing.org or QRStuff to decode and verify the destination of QR code.

🔐 Recommendations
Do Not Scan QR Code in suspicious emails.

Verify refund claims directly with IRCTC or your service provider via official channels.

Report such emails to your IT department or CERT-In (Indian Computer Emergency Response Team).

Implement email gateway filters with SPF, DKIM, and DMARC enforcement.

🧾 Conclusion
This email is a clear phishing attempt using social engineering, QR code obfuscation, and urgency. Awareness and technical safeguards are key to avoiding such scams.
