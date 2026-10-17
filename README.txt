ESTHER WORLD — INTEGRATED GAME + ADMIN STARTER

Files: index.html (game bridge), admin.html/admin.js (admin UI), worker.js (Worker source), config.js (Worker URL).

The API Worker is deployed at https://esther-world-api.workers.dev and uses D1 database esther-world-db. The ADMIN_TOKEN secret is not yet configured, so admin endpoints will reject requests until it is added under Cloudflare Worker Settings > Variables and Secrets. Never place that secret in these public files.

Player IDs are per browser/device, not cross-device accounts. This starter supports admin-set token balances and global announcements; game-earned/spent coins are not securely synchronized across devices. Test before relying on it.
