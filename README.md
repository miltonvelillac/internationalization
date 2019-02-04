# Internationalization

* Para angular 6
- Instalar en este orden
- ng add @ngx-i18nsupport/tooling --i18nLocale=es --languages es,en
- npm install @ngx-translate/i18n-polyfill@1.0.0 --save
- npm i ngx-i18nsupport@0.16.3 --save

* You can specify the base locale of your app with the--i18n-locale command option:
- ng xi18n --i18n-locale es

* https://github.com/martinroob/ngx-i18nsupport/tree/master/projects/xliffmerge
* https://github.com/martinroob/ngx-i18nsupport/wiki/Tutorial-for-using-xliffmerge-with-angular-cli


# Build
ng build --prod --i18n-file src/i18n/messages.es.xlf --i18n-format xlf --i18n-locale es
ng build --prod --i18n-file src/i18n/messages.en.xlf --i18n-format xlf --i18n-locale en

ng build --prod --i18n-file src/i18n/messages.es.xlf --i18n-format xlf --i18n-locale es
ng build --aot --output-path dist/internationalization/en --prod --i18n-file src/i18n/messages.en.xlf --i18n-format xlf --i18n-locale en