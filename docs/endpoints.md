# Endpoints

## Authentication
- `POST /auth/google`
- `POST /auth/apple`
- `GET /auth/apple/callback`
- `POST /auth/authorize`
- `POST /auth/token`
- `POST /auth/revoke`
- `GET /profile/eula`
- `POST /permissions`

## Profile and account
- `GET /profile`
- `PATCH /profile/name`
- `PATCH /profile/username`
- `POST /profile/image`
- `POST /profile/banner`
- `GET /profile/followers?page=`
- `GET /profile/following?page=`
- `POST /firebase-token`
- `GET /verified-identity`

## Feed and posts
- `GET /v2/feed?limit=15`
- `GET /feed/`
- `POST /posts`
- `GET /recommended-users?page=`
- `GET /comments?limit=`
- `GET /comments`
- `GET /replies?limit=`
- `GET /replies`
- `POST /likes`
- `POST /reports`
- `GET /blocked`
- `GET /blockers`
- `POST /checkin`
- `GET /checkins?page=`

## Users and social graph
- `GET /users?search=`
- `GET /users/`
- `GET /followers`
- `GET /followers/stats`
- `GET /recommended-breeders?page=1&limit=6`
- `GET /recommended-strains?page=1&limit=6`
- `GET /admin/users/`
- `GET /admin/feed/`
- `GET /admin/comments/`
- `GET /admin/places/`

## Grower and market domain
- `GET /breeders?search=`
- `GET /breeders/`
- `GET /admin/breeders`
- `GET /strains?search=`
- `GET /strains/`
- `GET /admin/strains`
- `GET /claimables`
- `GET /claimables/`
- `GET /claimers`
- `GET /holders`
- `GET /products/`
- `GET /market/users/`
- `GET /places/`
- `GET /address-verification`

## Notifications and chat
- `GET /notifications/count`
- `GET /v2/notifications?limit=15`
- `GET /chats?limit=15`
- `GET /chats/stats`
- `GET /messages?limit=`

## Media
- `POST /media`
- `POST /media-orientation`
- `GET /banner`
- `POST /profile-image`
- `GET /image`
- `GET /videos`

## Gamification
- `GET /badges`
- `GET /custom-badges?page=`

## Discovery and admin
- `GET /recommendations`
- `GET /feature`
- `GET /features`
- `GET /reports`

## Other
- `POST /trk`
