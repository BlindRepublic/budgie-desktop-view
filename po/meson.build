i18n = import('i18n')

# for i in *.po; do echo "    '$i'," | sed 's/\.po//'; done
langs = [
    'cs',
    'en_GB',
    'en_US',
    'es',
    'es_MX',
    'fr',
    'he',
    'ja',
    'ja_JP',
    'ko',
    'lt',
    'ms_MY',
    'pt_BR',
    'pt_PT',
    'ru',
    'sq',
    'tr',
    'uk',
    'vi_VN',
    'zh',
    'zh_CN',
]

# Stole this from gnome-twitch, ty TingPing
# https://github.com/vinszent/gnome-twitch/tree/master/po
i18n.gettext(meson.project_name(), languages : langs, args : [
    '--from-code=UTF-8',
    '--add-comments',
    '--package-name=' + meson.project_name(),
    '--package-version=' + meson.project_version(),
    '--keyword=_',
    '--keyword=N_',
    '--keyword=C_:1c,2',
    '--keyword=NC_:1c,2',
    '--keyword=g_dcgettext:2',
    '--keyword=g_dngettext:2,3',
    '--keyword=g_dpgettext2:2c,3',

    '--flag=N_:1:pass-c-format',
    '--flag=C_:2:pass-c-format',
    '--flag=NC_:2:pass-c-format',
    '--flag=g_dngettext:2:pass-c-format',
    '--flag=g_strdup_printf:1:c-format',
    '--flag=g_string_printf:2:c-format',
    '--flag=g_string_append_printf:2:c-format',
    '--flag=g_error_new:3:c-format',
    '--flag=g_set_error:4:c-format',
])
