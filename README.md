# BACKEND
Skip to content
Navigation Menu
franciswagonda
Backend-

Code
Issues
Pull requests
Actions
Projects
Wiki
Security
Insights
Settings
Commit 4a7d6cf
franciswagonda
franciswagonda
committed
	new file:   .env.example
	renamed:    backend/.gitignore -> .gitignore
	renamed:    backend/README.md -> README.md
	renamed:    backend/analyze_colors.js -> analyze_colors.js
	deleted:    backend/EMAIL_SETUP.md
	deleted:    backend/seed.js
	renamed:    backend/controllers/authController.js -> controllers/authController.js
	renamed:    backend/controllers/dashboardController.js -> controllers/dashboardController.js
	renamed:    backend/controllers/facultyController.js -> controllers/facultyController.js
	renamed:    backend/controllers/projectController.js -> controllers/projectController.js
	renamed:    backend/controllers/userController.js -> controllers/userController.js
	renamed:    backend/docs/working-theories.md -> docs/working-theories.md
	renamed:    backend/middleware/authMiddleware.js -> middleware/authMiddleware.js
	renamed:    backend/middleware/uploadMiddleware.js -> middleware/uploadMiddleware.js
	renamed:    backend/models/Comment.js -> models/Comment.js
	renamed:    backend/models/Department.js -> models/Department.js
	renamed:    backend/models/Faculty.js -> models/Faculty.js
	renamed:    backend/models/Project.js -> models/Project.js
	renamed:    backend/models/ProjectView.js -> models/ProjectView.js
	renamed:    backend/models/User.js -> models/User.js
	renamed:    backend/models/index.js -> models/index.js
	renamed:    backend/package-lock.json -> package-lock.json
	renamed:    backend/package.json -> package.json
	renamed:    backend/routes/authRoutes.js -> routes/authRoutes.js
	renamed:    backend/routes/dashboardRoutes.js -> routes/dashboardRoutes.js
	renamed:    backend/routes/facultyRoutes.js -> routes/facultyRoutes.js
	renamed:    backend/routes/projectRoutes.js -> routes/projectRoutes.js
	renamed:    backend/routes/userRoutes.js -> routes/userRoutes.js
	new file:   seed.js
	renamed:    backend/server.js -> server.js
	new file:   uploads/document-1764167971777.pdf
1 parent 
3d3f68e
 commit 
4a7d6cf
File tree
Filter files…
.env.example
.gitignore
README.md
analyze_colors.js
backend
EMAIL_SETUP.md
seed.js
controllers
authController.js
dashboardController.js
facultyController.js
projectController.js
userController.js
docs
working-theories.md
middleware
authMiddleware.js
uploadMiddleware.js
models
Comment.js
Department.js
Faculty.js
Project.js
ProjectView.js
User.js
index.js
package-lock.json
package.json
routes
authRoutes.js
dashboardRoutes.js
facultyRoutes.js
projectRoutes.js
userRoutes.js
seed.js
server.js
uploads
document-1764167971777.pdf
31 files changed
+517
-282
lines changed
‎.env.example‎
+17
Lines changed: 17 additions & 0 deletions
Original file line number	Diff line number	Diff line change
@@ -0,0 +1,17 @@
PORT=5000
DB_NAME=ucu_innovators
DB_USER=root
DB_PASSWORD=your_password_here
DB_PORT=3306
DB_HOST=localhost
JWT_SECRET=your_jwt_secret_here
# Email Configuration for Password Reset
# For Gmail: Use App Password (https://support.google.com/accounts/answer/185833)
# For other providers: Check their SMTP settings
SMTP_HOST=smtp.gmail.com
SMTP_PORT=587
SMTP_USER=your-email@gmail.com
SMTP_PASS=your-app-password
SMTP_FROM=UCU Innovators Hub <noreply@ucu.ac.ug>
FRONTEND_URL=http://localhost:5173
‎backend/.gitignore‎ renamed to ‎.gitignore‎
+2
Lines changed: 2 additions & 0 deletions
Original file line number	Diff line number	Diff line change
@@ -2,3 +2,5 @@
.env

node_modules/
EMAIL_SETUP.md
‎backend/README.md‎ renamed to ‎README.md‎


File renamed without changes.
‎backend/analyze_colors.js‎ renamed to ‎analyze_colors.js‎
File renamed without changes.
‎backend/EMAIL_SETUP.md‎
-123
Lines changed: 0 additions & 123 deletions
This file was deleted.
‎backend/seed.js‎
-106
Lines changed: 0 additions & 106 deletions
This file was deleted.
0 commit comments
Comments
0
 (0)
Footer
© 2025 GitHub, Inc.
Footer navigation
Terms
Privacy
Security
Status
Community
Docs
Contact
Manage cookies
Do not share my personal information
