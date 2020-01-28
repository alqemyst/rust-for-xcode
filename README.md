# Installation
Directories Plug-ins, Specifications, Templates from repo should be copied or merged to ~/Library/Developer/Xcode/

As of Xcode 11 syntaxes no longer work with Specifications directory. We need two additional commands after each Xcode update.

```sh
sudo cp ~/Library/Developer/Xcode/Specifications/Xcode.SourceCodeLanguage.Rust.plist /Applications/Xcode.app/Contents/SharedFrameworks/SourceModel.framework/Versions/A/Resources/LanguageMetadata/

sudo cp ~/Library/Developer/Xcode/Specifications/Rust.xclangspec /Applications/Xcode.app/Contents/SharedFrameworks/SourceModel.framework/Versions/A/Resources/LanguageSpecifications/
```

# Project template
Build system runs cargo $(ARGS). If needed Debug and Release can have their own values (e.g. build --release for Release).

# Supported UUIDs
`2FD51EF8-522D-4532-9698-980C4C497FD1`
`92CB09D8-3B74-4EF7-849C-99816039F0E7`
`A74FBA51-FFEA-4409-B976-6FC3225A6F64`
`BAB79788-ACEE-4291-826B-EC4667A6BEC5`
