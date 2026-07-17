# Sur AI Music - Build Instructions

## Project Structure
এটি একটি মাল্টি-মডিউল Android গ্রেডল প্রজেক্ট:

### মডিউলগুলো:
- **app** - প্রধান অ্যাপ্লিকেশন
- **core** - শেয়ার করা কম্পোনেন্ট এবং থিম
- **data** - ডেটা লেয়ার এবং রেপোজিটরি
- **domain** - বিজনেস লজিক এবং এন্টিটি
- **feature/** - ফিচার মডিউলগুলো:
  - auth - অথেন্টিকেশন
  - music - মিউজিক প্লেয়ার
  - lyrics - লিরিক্স
  - social - সোশ্যাল শেয়ারিং
  - marketplace - মার্কেটপ্লেস
  - admin - অ্যাডমিন প্যানেল
  - payment - পেমেন্ট সিস্টেম
  - settings - সেটিংস
  - video - ভিডিও প্লেয়ার

## প্রয়োজনীয় টুলস:
- JDK 11+ (প্রেফারেবলি 17)
- Android SDK 34+
- Gradle 8.0+

## বিল্ড কমান্ড:

### Debug Build:
```bash
./gradlew assembleDebug
```

### Release Build:
```bash
./gradlew assembleRelease
```

### সব টেস্ট রান করো:
```bash
./gradlew test
```

### এন্ড-টু-এন্ড টেস্ট:
```bash
./gradlew connectedAndroidTest
```

## লোকাল সেটআপ:

1. **local.properties তৈরি করো** (যদি না থাকে):
```properties
sdk.dir=/path/to/android/sdk
```

2. **ডিপেন্ডেন্সিগুলো ডাউনলোড করো**:
```bash
./gradlew build --dry-run
```

3. **প্রজেক্ট বিল্ড করো**:
```bash
./gradlew build
```

---
**Generated**: This project was extracted from SurProAIMusic.zip
