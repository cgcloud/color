cmake_minimum_required(VERSION 2.8)

include(RezBuild)

file(GLOB lut_files "luts/*")

rez_install_files(
    ${lut_files}
    DESTINATION .
)

rez_install_files(
    package.yaml
    DESTINATION .
)

rez_install_files(
    config.ocio
    DESTINATION .
)

