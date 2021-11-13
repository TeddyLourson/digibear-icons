# Update process

1. Save all the icons under icons/{style}
2. Run `yarn clean-up` to clean up the icons.
3. Use the generate-json-metadata plugin in figma and save the json file
under release/{versionNumber}
4. Move into the release with `cd release/{versionNumber}`
5. Zip the content with `zip digibear-icons.zip -r ./`
6. Create a github release with `gh release create v{versionNumber} ./digibear-icons.zip`
7. Rebuild the other plugins.