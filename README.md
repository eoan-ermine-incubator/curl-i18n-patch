# curl-i18n

Patches for curl that add internationalization support for libcurl error messages.

Install `curl-i18n`, then install the localization package for each language you need (see https://github.com/eoan-ermine/curl-l10n). Once installed, `curl_easy_strerror` will return error messages in the language specified by the current locale.

## Installation

1. Clone the curl repository:

```
git clone git@github.com:curl/curl.git
cd curl
```

2. Check out a supported version (for example, 8.16.0):

```
git checkout curl-8_16_0
```

3. Download and apply the patch for the selected version:

```
wget -qO - https://raw.githubusercontent.com/eoan-ermine-incubator/curl-i18n-patch/refs/heads/$(git describe)/curl-i18n.patch | git apply
```

4. Build and install curl according to the [curl official documentation](https://curl.se/docs/install.html). 