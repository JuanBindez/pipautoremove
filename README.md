# pipautoremove
auto remove pip list

    for /f "delims=" %i in ('pip freeze ^| findstr /v "^pip==^"') do pip uninstall -y %i
