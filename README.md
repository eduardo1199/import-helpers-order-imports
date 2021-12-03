#Import-helpers-order-imports

##Install dev dependecies 

yarn add eslint-plugin-import-helpers -D

##Config

 rules: {
    'import-helpers/order-imports': [
      'error',
      { 
          newlinesBetween: 'always',
          groups: [
              '/^react/',
              'module',
              '/^@/',
              '/^hooks/',
              '/^services/',
              '/^models/',
              '/^utils/',
              '/^pages/',
              '/^components/',
              '/^./components/',
              '/^./state/',
              '/^./utils/',
              ['parent', 'sibling', 'index'],
          ],
          alphabetize: { ignoreCase: true },
      }
    ],
  },
