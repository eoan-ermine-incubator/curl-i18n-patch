# curl-i18n

Patches for curl that add internationalization support for libcurl error messages.

Install `curl-i18n`, then install the localization package for each language you need (see https://github.com/eoan-ermine/curl-l10n). Once installed, `curl_easy_strerror` will return error messages in the language specified by the current locale.
