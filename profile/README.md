# Project 3 Group 6

## Description
Users pin and review spots that aren't on mainstream apps like secret study spots, less popular food spots, scenic views near campus, etc. All locations created by users (or admin).

## Tech Stack
- OAuth2
- Supabase
- JWT utilities
- Docker
- Render
- Spring Boot
- Postman
- JUnit

## How to Run
*Login/Auth
User Profiling

*Setup Account setting and prefernces

*Geospatial search with filtering

*Approve, feature, or remove locations

*Submit reviews with star ratings

*Follow/Unfollow other users

*View public profiles

*Check out activity feed

Favorites/Following

## Important Commands
### Run Backend
- Our backend is containerized with Docker, and can be built and run with the following command
```bash
docker build -t hiddengems-backend .
docker run --env-file .env -p 8080:8080 hiddengems-backend .
```

### Run Frontend
- We use Expo (React Native) for both our web and mobile frontends, you can run both with
```bash
npx expo start
```

- Alternatively, flags can be used to only run a specific version of the frontend
```bash
npx expo start -w
npx expo start --web //web

npx expo start -a
npx expo start --android //android
```

### Run tests
- in /frontend (jest)
```bash
npm test -- --coverage --coverageReporters=text --coverageDirectory=none
```

## Hosting
- Backend hosted with Render at https://backend-vjot.onrender.com/