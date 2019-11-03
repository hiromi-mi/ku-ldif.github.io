# ku-ldif.github.io

Kyoto University LDIF Daisuki Club (ja: 京都大学 LDIF 同好会) <https://ku-ldif.github.io/>

This project uses [ldap2html](https://github.com/nonylene/ldap2html) for converting LDIF to html.

## Guide

### Add documents

LDIF files (`*.html.ldif`) under the `src` directory will be passed to `ldapadd`.

### Modify documents

**DON'T MODIFY LDIF, DO ADD NEW LDIF.**

If you want to modify existing docuemnts, use `ldapmodify`.

LDIF files (`XXX-*.html.ldif`) under the `src/modify` directory will be passed to `ldapmodify` in alphabetical order, after all `ldapadd`s.

### Note

For now, one commit after ku-ldif's commit is needed to deploy GitHub pages ([issue](https://github.com/ku-ldif/ku-ldif.github.io/issues)).

## License

See [LICENSE](./LICENSE).
