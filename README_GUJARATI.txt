MDM Offline Android App - Starter v0.1

આ શું છે?
- ગુજરાતી ભાષામાં offline Android WebView app નો starter code.
- MDM માટે પ્રતિ વિદ્યાર્થી ગ્રામથી કિલોગ્રામ ગણતરી.
- IFMS/PFMS માટે સરળ voucher entry અને local record storage.
- CSV export.

મહત્વની મર્યાદા:
આ હજી prototype છે. Excelની તમામ merged cells, formulas, grant-wise ratios, original voucher print layouts અને ખર્ચની બધી વિગત તેમાં હજી port કરેલી નથી. MDM ગ્રામના fields demo values છે; સત્તાવાર મેનુ/Excel પ્રમાણે ચકાસ્યા વગર ન વાપરશો. આ prototype ને સત્તાવાર હિસાબ માટે વાપરતા પહેલાં દરેક total ને Excel સામે test કરો.

APK build કરવાની સરળ રીત (Windows 7, 2 GB RAM માટે):
1. આ ZIP ને GitHub પર નવી repositoryમાં upload કરો (browser દ્વારા).
2. Repository → Actions tab ખોલો.
3. “Build offline Android APK” workflow પસંદ કરો → Run workflow.
4. Build સફળ થાય પછી workflow run માં Artifacts વિભાગમાંથી MDMOffline-debug-apk.zip download કરો.
5. ZIP ખોલો; app-debug.apk Android phone પર મોકલો.
6. ફોનમાં APK ખોલીને install કરો. જો પૂછે તો માત્ર આ file manager/browser માટે “Install unknown apps” મંજૂરી આપો.

નોંધ:
- Build માટે GitHub account/internet જરૂરી છે; app પોતે offline ચાલે તે રીતે બનાવેલી છે.
- GitHub Actions interface અથવા Android SDK બદલાય તો build workflowમાં ફેરફારની જરૂર પડી શકે.
- Debug APK testing માટે છે; public distribution માટે signed release APK બનાવવી પડશે.
- LocalStorageમાં રહેલા રેકોર્ડ app data clear/uninstall કરવાથી ગુમાઈ શકે છે. CSV exportથી backup રાખો.
