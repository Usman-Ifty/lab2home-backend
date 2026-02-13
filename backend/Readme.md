# Lab2Home - Backend API Engine

The robust server-side engine powering the Lab2Home healthcare ecosystem. This API manages diagnostic bookings, marketplace transactions, real-time communications, and secure payment processing.

## 🛠️ Core Technology Stack
- **Runtime**: Node.js & Express.js
- **Database**: MongoDB Atlas (via Mongoose ODM)
- **Real-time**: Socket.io for live notifications and clinician-patient chat
- **Payment**: PayFast Integration (Signature validation & ITN Webhooks)
- **Email**: Nodemailer (SMTP Service)
- **Language**: TypeScript for type-safe development

## 📁 Key Modules
- `/src/controllers`: Request handling and core business logic
- `/src/models`: Mongoose schemas with built-in data validation
- `/src/routes`: Organized RESTful API endpoints
- `/src/services`: External integrations (PayFast SDK, Email templates)
- `/src/socket`: WebSocket event handlers for real-time status updates

## ⚙️ Deployment & Environment
This backend is optimized for deployment on cloud platforms like **Render** or **Railway**.

### Build & Run Commands:
- **Build**: `npm install && npm run build`
- **Start**: `npm start`
- **Development**: `npm run dev`

### Mandatory Environment Variables:
Ensure these are configured in your deployment platform settings (Render Dashboard):
- `MONGODB_URI`: Your MongoDB Atlas connection string
- `JWT_SECRET`: Secure key for token generation
- `PAYFAST_MERCHANT_ID`: Your PayFast merchant identifier
- `PAYFAST_MERCHANT_KEY`: Your PayFast merchant key
- `PAYFAST_PASSPHRASE`: Secure signature salt

## 🔒 Security Compliance
- Fully integrated with PayFast signature verification.
- ITN (Instant Transaction Notification) webhooks for secure payment confirmation.
- Cross-Origin Resource Sharing (CORS) protection for frontend security.

## 📄 Project Governance
Final Year Project (FYP-II) - Lab2Home Development Team.
- **Supervised by**: Mahzaib Younus
- **Lead Developers**: Muhammad Usman Awan, Faizan Ahmad, Muhammad Ahmad