
---

## 🔹 Frontend

### Project Structure

```
src/
├─ components/
├─ pages/
└─ main.jsx
public/
.env
package.json
```

---

### Features

* Connects to backend API
* Displays campaigns and recipient management
* Allows merchants to schedule SMS/email

---

### Environment Variables

Create a `.env` file:

```env
VITE_API_BASE_URL=http://localhost:3000
```

> Replace with deployed backend URL for production

---

### Run Frontend

```bash
npm install
npm run dev
```

Frontend runs at:

```
http://localhost:5173
```

---

### Deployment (Netlify)

1. Connect repository to Netlify
2. Add environment variable:

```
Key:   VITE_API_BASE_URL
Value: https://your-backend-domain
```

3. Redeploy site

---

### Resources

* BullMQ — [https://docs.bullmq.io/](https://docs.bullmq.io/)
* Redis — [https://redis.io/](https://redis.io/)
* MongoDB — [https://www.mongodb.com/](https://www.mongodb.com/)
* Resend — [https://resend.com](https://resend.com)
* Nodemailer — [https://nodemailer.com/](https://nodemailer.com/)

---

### Contribution

* Use Nodemailer locally
* Use Resend or any email API in production
* Replace the email layer entirely if needed

Open issues or submit pull requests 🚀

---