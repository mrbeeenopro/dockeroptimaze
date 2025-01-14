# dockeroptimaze
optimaze docker for pteroactyl


for <4gb ram 

`java 8 dragonwell|ghcr.io/trenutoo/pterodactyl-images:java_8_dragonwell`

`java 11 dragonwell|ghcr.io/trenutoo/pterodactyl-images:java_11_dragonwell`

`java 17 dragonwell|ghcr.io/trenutoo/pterodactyl-images:java_17_dragonwell`

`java 21 dragonwell|ghcr.io/trenutoo/pterodactyl-images:java_21_dragonwell`

you can use dragonwell for sppedup starup

for 6-<8gb ram yolks is good u dont have to chagne

for big server >16gb ram up

`java 8 graalvm|ghcr.io/trenutoo/pterodactyl-images:java_8_graalvm`

`java 17 graalvm|ghcr.io/trenutoo/pterodactyl-images:java_11_graalvm`

`java 21 graalvm|ghcr.io/trenutoo/pterodactyl-images:java_21_graalvm`

`java 22 graalvm|ghcr.io/trenutoo/pterodactyl-images:java_22_graalvm`


starup basic

`java -Xms256M -Xmx$(({{SERVER_MEMORY}} - ({{SERVER_MEMORY}}/10)))M -XX:+UseG1GC -XX:+ParallelRefProcEnabled -XX:MaxGCPauseMillis=200 -XX:+UnlockExperimentalVMOptions -XX:+DisableExplicitGC -XX:G1NewSizePercent=30 -XX:G1MaxNewSizePercent=40 -XX:G1HeapRegionSize=8M -XX:G1ReservePercent=20 -XX:G1HeapWastePercent=5 -XX:G1MixedGCCountTarget=4 -XX:InitiatingHeapOccupancyPercent=15 -XX:G1MixedGCLiveThresholdPercent=90 -XX:G1RSetUpdatingPauseTimePercent=5 -XX:SurvivorRatio=32 -XX:+PerfDisableSharedMem -XX:MaxTenuringThreshold=1 -Dusing.aikars.flags=https://mcflags.emc.gs -Daikars.new.flags=true -jar {{SERVER_JARFILE}}`



goodluck =)
