# w10-zowe 
git clone https://TOKEN@github.com/drb1972/w10-zowe.git
 
## Instalación standard

- zowe v2 con CUST002 en Global Configuration

### Proceso
- Instalar Nodejs: https://nodejs.org/en/download
- Instalar VSCode: https://code.visualstudio.com/download 
- Instalar Git:  https://git-scm.com/download/win 
- Instalar ooRexx: https://sourceforge.net/projects/oorexx/ 
- Instalar Python: Desde Microsoft Store buscar Python 
- Instalar VSCode Extension para Python 

- Restart

### Instalar Zowe: https://docs.zowe.org/stable/getting-started/cli-getting-started
- npm install -g @zowe/cli@zowe-v2-lts
- zowe plugins install @zowe/cics-for-zowe-cli@zowe-v2-lts 
- zowe plugins install @zowe/db2-for-zowe-cli@zowe-v2-lts 
- zowe plugins install @zowe/ims-for-zowe-cli@zowe-v2-lts 
- zowe plugins install @zowe/mq-for-zowe-cli@zowe-v2-lts 
- zowe plugins install @zowe/zos-ftp-for-zowe-cli@zowe-v2-lts
- Instalar Extension Code4z

Copiar zowe.config.json y zowe.schema.json a C:\Users\root\.zowe 

Para cambiar de profile: 
zowe config set "defaults.zosmf" "LPAR.zosmf" --gc

Ejemplo de comando con profile zowe files list ds cust002.* --zosmf-profile LPAR.zosmf siendo LPAR mstr o sr01


