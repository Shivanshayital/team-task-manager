# Railpack Deployment Fix - TODO

## [x] Step 1: Create/Update root package.json with start script delegating to server/
- Added `\"scripts\": {\"start\": \"cd server && npm start\", \"dev\": \"cd server && npm run dev\"}, \"main\": \"server/server.js\", \"type\": \"module\".

## [x] Step 2: Merged deps to root package.json, npm ci now works for Railway

## [ ] Step 3: Test locally
```bash
npm start
```
Expected: Server running on port 5000. Test `curl http://localhost:5000/api/health` or browser.

## [ ] Step 4: Redeploy to Railpack platform.

## [ ] Step 5: Verify full app (frontend + backend)
- Backend: `npm start`
- Frontend: New terminal `cd client && npm install && npm run dev` (proxies to :5000)

**Next**: Run suggested commands and redeploy.
