# TEST-RUB – Firebase & EAS Dev Client test  
Dette projekt er en simpel test-app lavet i React Native med Expo og Firebase, hvor jeg afprøvede EAS Build og Dev Client for første gang. Appen indeholder kun login og opret bruger, og blev brugt til at teste emulatoropsætning og Firebase-auth i Dev Client-miljø.

## Teknologier brugt
- React Native (Expo)
- Firebase (Authentication)
- EAS Build og Dev Client
- React Navigation
- JavaScript (JSX)
- Android Emulator (via Android Studio)
- Visual Studio Code

## Funktioner
- Login med e-mail og adgangskode (Firebase)
- Opret bruger med Firebase-auth
- Enkel navigation mellem login og tilmeld
- Brug af EAS Dev Client i stedet for Expo Go

## Sådan kører du projektet på din egen computer
### 1. Installer Node.js
   
Download og installer Node.js fra https://nodejs.org
(Node.js indeholder også npm, som vi skal bruge)

### 2. Installer Expo CLI og EAS CLI
```bash
npm install -g expo-cli eas-cli
```

### 3. Klon projektet fra Github

```bash
git clone https://github.com/saebir/GammelRUB.git
cd F-rste-Login
```

### 4. Installer projektets afhængigheder

```bash
npm install
```

### 5. Byg med EAS og start Dev Client

```bash
eas build --profile development --platform android
```

Når buildet er færdigt, installer .apk-filen i emulator eller på en fysisk enhed (via adb install).

### 6. Start derefter appen i Dev Client:

```bash
npx expo start --dev-client
```

### Emulatortip:
Hvis emulatoren ikke åbner:

```bash
emulator -list-avds
emulator -avd <navn_på_emulator> -gpu swiftshader_indirect
npx expo start --dev-client
```

## Status
Projektet er ikke færdigt, men fungerede som teknisk test. Enkelte dele af koden er senere blevet genbrugt i det fulde "Rock under Broen"-projekt.
