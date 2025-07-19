# Project Export Checklist

## Essential Files to Export

### Root Level

- [ ] package.json
- [ ] package-lock.json (if exists)
- [ ] tsconfig.json
- [ ] tailwind.config.ts
- [ ] vite.config.ts
- [ ] vite.config.server.ts
- [ ] postcss.config.js
- [ ] components.json
- [ ] index.html
- [ ] netlify.toml
- [ ] SETUP_GUIDE.md
- [ ] EXPORT_CHECKLIST.md

### Client Folder (Frontend)

- [ ] client/App.tsx
- [ ] client/global.css
- [ ] client/vite-env.d.ts

#### Components

- [ ] client/components/Charts.tsx
- [ ] client/components/Layout.tsx
- [ ] client/components/RealTimeTracker.tsx
- [ ] client/components/ui/ (entire folder with all 44 UI components)

#### Contexts

- [ ] client/contexts/ThemeContext.tsx

#### Hooks

- [ ] client/hooks/use-mobile.tsx
- [ ] client/hooks/use-toast.ts
- [ ] client/hooks/useRealtimeData.ts

#### Pages

- [ ] client/pages/Analytics.tsx
- [ ] client/pages/Apps.tsx
- [ ] client/pages/Data.tsx
- [ ] client/pages/Index.tsx
- [ ] client/pages/NotFound.tsx
- [ ] client/pages/System.tsx
- [ ] client/pages/Tracker.tsx

#### Lib

- [ ] client/lib/utils.ts
- [ ] client/lib/utils.spec.ts

### Server Folder (Backend)

- [ ] server/index.ts
- [ ] server/node-build.ts
- [ ] server/routes/demo.ts
- [ ] server/routes/tracker.ts

### Shared Folder

- [ ] shared/api.ts

### Public Folder

- [ ] public/placeholder.svg
- [ ] public/robots.txt

### Netlify Functions

- [ ] netlify/functions/api.ts

## Post-Export Steps

1. **Create new folder** on your local machine
2. **Copy all files** maintaining exact folder structure
3. **Open folder in VS Code**
4. **Run setup commands**:
   ```bash
   npm install
   npm run dev
   ```

## Verification

After setup, you should see:

- ✅ Development server running on http://localhost:5173
- ✅ No TypeScript errors
- ✅ All pages accessible via sidebar navigation
- ✅ Charts rendering properly
- ✅ Theme toggle working
- ✅ Responsive design on mobile/desktop

## Important Notes

- **Keep folder structure identical** to cloud environment
- **Don't modify package.json** during export
- **Include all hidden files** if any exist
- **Verify all import paths** work correctly after export
