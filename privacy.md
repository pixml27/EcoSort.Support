---
layout: page
title: Privacy Policy
description: AI-powered recycling assistant
---

<body>

    <div class="container">
        
        <header class="page-header">
            <a href="index.html" class="back-link">← Back to Home</a>
        </header>

        <main class="privacy-content">
            <h1>Privacy Policy for EcoSort</h1>

            <div class="meta-info">
                <p><strong>Effective Date:</strong> June 24, 2025</p>
                <p><strong>Last Updated:</strong> October 26, 2025</p>
            </div>

            <h2>1. Introduction</h2>
            <p>Welcome to EcoSort! This Privacy Policy describes how Arsenii Koriaigin ("we," "us," or "our") collects, uses, processes, and safeguards your information when you use our mobile application, EcoSort (the "App").</p>
            <p>EcoSort helps users identify the correct waste disposal category based on photos and provides recommendations according to local recycling rules in supported countries: Spain, Portugal, Italy, Austria, France, Germany, and the Netherlands.</p>
            <p>We are committed to protecting your privacy and handling your data in accordance with the General Data Protection Regulation (GDPR). By using EcoSort, you agree to the practices described in this Privacy Policy.</p>
            <p>This Privacy Policy is available in multiple languages within the App.</p>

            <h2>2. Data Controller</h2>
            <p>The data controller responsible for your personal data is:</p>
            <p>Arsenii Koriaigin<br>
            <a href="mailto:akor@ecosort.app">akor@ecosort.app</a><br>
            Barcelona, Spain</p>

            <h2>3. What Information We Collect and Why</h2>
            <p>We collect minimal information necessary to operate and improve the App.</p>

            <h3>a) Image Data (Photos from Camera or Gallery)</h3>
            <ul>
                <li><strong>How it's collected:</strong> The App captures photos using your device's camera or allows you to select images from your device's gallery when you choose to use the image classification feature.</li>
                <li><strong>What is collected:</strong> The image file (temporarily stored as an <code>XFile</code> object).</li>
                <li><strong>Processing:</strong> Images are processed on your device to be resized and compressed before being sent for AI analysis using Google's API.</li>
                <li><strong>Purpose:</strong> To identify the correct waste disposal bin and provide local recycling instructions.</li>
                <li><strong>Storage & Retention:</strong> Images are not permanently stored on your device or our servers. They are used only for the immediate classification request and then discarded.</li>
                <li><strong>Legal Basis for Processing:</strong> Your explicit <strong>consent</strong>. You are required to acknowledge this Privacy Policy before accessing camera functionalities for the first time.</li>
            </ul>

            <h3>b) User Account and Authentication Data</h3>
            <ul>
                <li><strong>How it's collected:</strong> When you register, sign in, or continue as an anonymous user.</li>
                <li><strong>What is collected:</strong> uid, email (if provided), emailVerified, isAnonymous, isPro, monthScanCount, ScanCount, monthScanLimit, createdAt, firstScanMonthPeriod, lastScanMonthPeriod, proStartMonthPeriod, proLastMonthPeriod, proSubscriptionsCount, and optionally sex and dateOfBirth.</li>
                <li><strong>Purpose:</strong> To manage user access, scan limits, and premium features, and to provide a consistent experience across sessions.</li>
                <li><strong>Storage:</strong> Stored securely in Firebase Firestore.</li>
                <li><strong>Retention:</strong> Until account deletion or 12 months of inactivity.</li>
                <li><strong>Legal Basis for Processing:</strong> Performance of a contract (to provide App functionality), legitimate interest (to maintain fair usage), and consent (for optional data).</li>
            </ul>

            <h3>c) Scan Records</h3>
            <ul>
                <li><strong>How it's collected:</strong> Automatically when you perform a classification.</li>
                <li><strong>What is collected:</strong> userId, scanId, createdAt, scan_country, scan_language, bin_color_english, and additional_instructions returned by the AI.</li>
                <li><strong>Purpose:</strong> To display results, manage usage limits, and improve system reliability.</li>
                <li><strong>Storage:</strong> Stored in Firestore; used for service analytics and troubleshooting, not for profiling.</li>
                <li><strong>Retention:</strong> Up to 12 months, after which data may be anonymized.</li>
                <li><strong>Legal Basis for Processing:</strong> Legitimate interest and performance of a contract.</li>
            </ul>

            <h3>d) Language and Country Settings</h3>
            <ul>
                <li><strong>How it's collected:</strong> When you choose your preferred language or country in the App.</li>
                <li><strong>What is collected:</strong> Language code (e.g., 'en', 'es', 'fr', 'ru', 'zh') and country code (e.g., 'ES', 'PT', 'IT').</li>
                <li><strong>Storage:</strong> Stored locally on your device.</li>
                <li><strong>Purpose:</strong> To display localized content and recommendations relevant to your region.</li>
                <li><strong>Retention:</strong> Persist until you change it or clear app data.</li>
                <li><strong>Legal Basis for Processing:</strong> Legitimate interest in usability and localization.</li>
            </ul>

            <h3>e) API Usage Tracking (Rate Limiting)</h3>
            <ul>
                <li><strong>How it's collected:</strong> Automatically when you use the classification feature.</li>
                <li><strong>What is collected:</strong> Local counters for number of scans and timestamps for each usage period.</li>
                <li><strong>Storage:</strong> Stored locally on your device.</li>
                <li><strong>Purpose:</strong> To prevent abuse and maintain fair use limits.</li>
                <li><strong>Retention:</strong> Automatically reset after the relevant time period (minute/day).</li>
                <li><strong>Legal Basis for Processing:</strong> Legitimate interest in maintaining service stability.</li>
            </ul>

            <h2>4. How We Use Your Information</h2>
            <p>We use collected data to:</p>
            <ul>
                <li>Provide App functionality (classification, recommendations, account management).</li>
                <li>Maintain fair use limits and prevent misuse.</li>
                <li>Improve reliability and ensure compliance with applicable recycling regulations.</li>
                <li>Comply with legal obligations.</li>
            </ul>
            <p>We do not sell or share your personal data for advertising or marketing purposes.</p>
            
            <h2>5. Data Sharing and Third Parties</h2>

            <h3>a) Firebase (Google Cloud Platform)</h3>
            <p>We use Firebase Authentication, Firestore Database, and Firebase Cloud Functions to securely manage user accounts, process classification requests, and handle backend logic. Google acts as a data processor under our instructions and in accordance with GDPR.</p>
            <p><strong>Cloud Functions & Logging:</strong> Firebase Cloud Functions may temporarily log technical information such as execution time, error codes, and IP address in an anonymized form for debugging and security monitoring. These logs are automatically deleted within 30 days.</p>
            <p>Learn more: <a href="https://firebase.google.com/support/privacy">https://firebase.google.com/support/privacy</a></p>

            <h3>b) Google's AI API</h3>
            <p>To provide image classification, we send compressed images to Google's AI API. No personal identifiers (UID, email, IP address) are included. Google acts as a data processor, handling requests per our instructions and applicable privacy agreements.</p>

            <h3>c) Other Third Parties</h3>
            <p>We do not share your personal data with other third parties except as required by law or to comply with legal obligations.</p>
            
            <h2>6. Data We DO NOT Collect</h2>
            <p>EcoSort does not collect or store:</p>
            <ul>
                <li>GPS or precise location data.</li>
                <li>Device identifiers (IMEI, MAC address, advertising ID).</li>
                <li>Behavioral analytics or tracking cookies.</li>
                <li>Contacts, messages, or other personal data stored on your device.</li>
            </ul>
            <p>We do not use personalized tracking or advertising SDKs.</p>

            <h2>7. Data Retention</h2>
            <p>We retain your data only as long as necessary to fulfill the purposes outlined in this Privacy Policy:</p>
            <ul>
                <li><strong>Image Data:</strong> Not stored.</li>
                <li><strong>User Account Data:</strong> Until account deletion or 12 months of inactivity.</li>
                <li><strong>Scan Records:</strong> Up to 12 months, then anonymized.</li>
                <li><strong>Cloud Function Logs:</strong> Up to 30 days, automatically deleted.</li>
                <li><strong>Language and API Tracking Data:</strong> Stored locally until you clear app data.</li>
            </ul>

            <h2>8. Data Security</h2>
            <p>We implement technical and organizational measures to protect your data, including HTTPS encryption, Firebase security rules, and access controls. Image processing occurs on your device before transmission. However, no method of data transmission over the Internet is 100% secure.</p>

            <h2>9. Data Processing Location</h2>
            <ul>
                <li><strong>On-device:</strong> language and country preferences, rate limit tracking, and image preprocessing.</li>
                <li><strong>Firebase (Google Cloud):</strong> account data, scans, and backend functions.</li>
                <li><strong>Google AI API:</strong> image classification.</li>
            </ul>
            <p>Data may be processed on servers located outside your country, including in the European Union and the United States.</p>

            <h2>10. International Data Transfers</h2>
            <p>Data processed through Firebase and Google AI may be transferred outside the European Economic Area (EEA). Google applies Standard Contractual Clauses (SCCs) and other appropriate safeguards to ensure GDPR compliance.</p>

            <h2>11. Your Rights Under GDPR</h2>
            <p>You have the right to:</p>
            <ul>
                <li>Be informed about how your data is used.</li>
                <li>Access and obtain a copy of your data.</li>
                <li>Rectify inaccurate or incomplete data.</li>
                <li>Request erasure of your data ("right to be forgotten").</li>
                <li>Restrict or object to certain processing.</li>
                <li>Request data portability.</li>
                <li>Withdraw consent at any time.</li>
            </ul>
            <p>To exercise your rights, contact us at <a href="mailto:akor@ecosort.app">akor@ecosort.app</a>. We will respond within one month as required by GDPR.</p>

            <h2>12. Children's Privacy</h2>
            <p>EcoSort is not intended for users under the age of 16. We do not knowingly collect data from children. If we become aware that a child has provided personal information, we will delete it promptly.</p>

            <h2>13. Disclaimer of Liability</h2>
            <p>EcoSort provides recycling guidance based on publicly available and municipal waste-sorting rules for supported countries. While we strive for accuracy, we cannot guarantee the completeness or correctness of all recommendations. EcoSort should not be relied upon as a legally binding or official source. Always verify with your local waste authority when in doubt.</p>

            <h2>14. Changes to This Privacy Policy</h2>
            <p>We may update this Privacy Policy from time to time. Updates will be posted within the App and indicated by an updated "Last Updated" date. Continued use of the App after changes constitutes acceptance of the revised Privacy Policy.</p>

            <h2>15. Contact Us</h2>
            <p>If you have any questions, concerns, or data-related requests, please contact us:</p>
            <p><a href="mailto:akor@ecosort.app">akor@ecosort.app</a></p>
            <p>Thank you for using EcoSort!</p>

        </main>
    </div>
</body>
