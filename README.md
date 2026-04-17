 Lab 14 - Lists & User Input

**Name:** Beksultan Kopzhasar
**Date:** 17.04.2026

---

## Task 1 - FlatList Contacts (Lab 14.1)

### Description
University Directory app with 100 mock contacts using FlatList virtualization.

### FlatList Optimizations
- `useCallback` — memoized renderItem and keyExtractor
- `getItemLayout` — fixed height items (80px) for mathematical positioning
- `initialNumToRender={15}` — initial render batch
- `maxToRenderPerBatch={10}` — items per render batch
- `windowSize={5}` — number of screens kept in memory
- `removeClippedSubviews={true}` — unmounts off-screen views

### Features
- Pull-to-refresh with RefreshControl
- Custom ListHeader and ItemSeparator
- 100 mock contacts generated dynamically

---

## Task 2 - Registration Form (Lab 14.2)

### Description
Registration form with keyboard handling and real-time email validation.

### Keyboard Handling
- `KeyboardAvoidingView` — iOS uses `padding`, Android uses `height`
- `TouchableWithoutFeedback` — dismisses keyboard on outside tap
- `keyboardVerticalOffset={64}` — offset for iOS status bar

### Form Validation
- Real-time email regex validation
- Error message shown for invalid email format
- Submit button disabled until email and password are filled
- `secureTextEntry` for password field
- `keyboardType="email-address"` for email field

---

## Folder Structure
```
Lab_14/
├── task1/
│   ├── src/
│   │   ├── screens/ContactsScreen.tsx
│   │   ├── utils/mockData.ts
│   │   └── types.ts
│   └── screenshots/
├── task2/
│   ├── src/
│   │   └── screens/RegistrationScreen.tsx
│   └── screenshots/
└── README.md
```