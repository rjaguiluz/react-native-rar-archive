# react-native-rar-archive

unrar for react native

## 🔧 Changes from the original version

- Removed TurboModules support to ensure compatibility with the classic React Native architecture.
- Modified RarArchive.h and RarArchive.mm for immediate usage in projects without the new architecture.

## Installation

```sh
npm install react-native-rar-archive
```

## Usage

```js
import { unrar } from 'react-native-rar-archive';
import { DocumentDirectoryPath } from 'react-native-fs';

// ...

const sourcePath = `${DocumentDirectoryPath}/archive.rar`;
const targetPath = `${DocumentDirectoryPath}/unrar`;

const result = await unrar(sourcePath, targetPath);
```

## Contributing

See the [contributing guide](CONTRIBUTING.md) to learn how to contribute to the repository and the development workflow.

## Native libraries used

- UnrarKit (ios) https://github.com/abbeycode/UnrarKit
- junrar (android) https://github.com/junrar/junrar

## License

MIT

---

Made with [create-react-native-library](https://github.com/callstack/react-native-builder-bob)
