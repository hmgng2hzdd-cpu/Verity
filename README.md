cd Website

# Delete wrong files
git rm app-page.js app-layout.js water-tracker.jsx

# Create correct structure and add files
mkdir -p app components
# Move/rename the files to correct locations
mv app-page.js app/page.js
mv app-layout.js app/layout.js
mv water-tracker.jsx components/WaterTracker.jsx

# Commit and push
git add .
git commit -m "Fix: Correct Next.js file structure"
git push origin main
