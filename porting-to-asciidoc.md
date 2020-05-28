$ gem install kramdown-asciidoc  

$ find ./ -name "*.md" -type f | xargs -I @@ \
    bash -c 'kramdoc --format=GFM --wrap=ventilate --output=@@.adoc @@';

$find . -type f -name '*.md' -delete
