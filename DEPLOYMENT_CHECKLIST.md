# Deployment checklist

- [ ] Push the complete project folder to a GitHub repository.
- [ ] In Render, create a Blueprint from that repository (`render.yaml`).
- [ ] Enter a strong `ADMIN_PASSWORD` when Render prompts for it.
- [ ] Wait until the PostgreSQL database and `oems` web service are deployed.
- [ ] Open `https://YOUR-RENDER-SERVICE.onrender.com/api/health` and confirm `{"status":"ok"}`.
- [ ] Open the service homepage and sign in as `admin` using the password entered during setup.
- [ ] Change the administrator password.
- [ ] Create schools, subjects, teacher accounts, student accounts, and examinations.
- [ ] Before real exams, use persistent database storage and verify backups/restore.

The frontend is served by the same Render service as the API. GitHub Pages is not used because it cannot host the Node.js API or PostgreSQL database.
