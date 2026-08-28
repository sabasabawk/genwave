# genwave
"GenWave — a general-audience social communication app connecting people through shared interests, conversations, and community."
## Target Audience
General audience — all ages, all backgrounds. Anyone looking to connect through shared interests rather than just existing friend circles.

## What Makes GenWave Different
GenWave connects people across generations and backgrounds through shared interests — not algorithms chasing endless scrolling, but real conversations and communities built around what people actually care about.

- Interest-first, not follower-first — you join based on what you love, not who's already famous
- Cross-generational — spaces where different age groups genuinely mix, instead of youth-only or professional-only spaces
- Conversation over content — less about posting for likes, more about real discussion and connection

## Key Features (MVP)
## Key Features (MVP — Version 1)
- User profiles
- Interest-based groups/communities

## Planned for Later Versions
- Posts / feed
- Messaging

## Monetization
- Freemium model: free to use, supported by ads (Google AdMob)
- Premium option: small subscription or one-time purchase to remove ads and unlock extra features (e.g. special profile badges, priority in interest groups)
- Future potential: in-app purchases for specific features as the app grows

## Status
Early concept stage — building out MVP definition before development begins.
## Screen Specs

### Profile Screen
- Profile photo
- Name
- Short bio (1-2 lines)
- Interests/tags (e.g. music, football, cooking) — connects users to relevant groups
- Location (optional — city/country only, not exact address)
- Viewable by other users (not just self)
### Groups Screen
- Users can create their own groups (any interest/topic)
- Each group has: name, description, category (e.g. Music, Sports, Cooking, Faith, Tech)
- Users find groups by browsing categories or searching by name/keyword
- Each group displays member count and a join button
## Data Structure (Firebase)

### users collection
- uid (auto-generated ID)
- name
- photoUrl
- bio
- interests (list/array)
- location (optional)

### groups collection
- groupId (auto-generated ID)
- name
- description
- category
- createdBy (uid of creator)
- memberCount

### group_members collection (tracks who joined which group)
- groupId
- uid
- joinedAt (date/time)