// SYNTAX TEST "Vue Component.sublime-syntax"

    <template>
// <- text.html.vue - text text
//  ^^^^^^^^^^ meta.tag.template.begin.html

    </template>
// <- text.html.vue - text text
//  ^^^^^^^^^^^ meta.tag.template.end.html

    </template><!-- stray template close tag -->
// <- text.html.vue - text text
//  ^^^^^^^^^^^ meta.tag.template.end.html

    <!--
    HAML Template Tests
    -->

    <template lang="haml">
//  ^^^^^^^^^^ meta.tag - meta.tag meta.tag - meta.attribute-with-value
//            ^^^^^^^^^^^ meta.tag meta.attribute-with-value.lang.html - meta.tag meta.tag
//                       ^ meta.tag.template.begin.html - meta.tag meta.tag
//  ^ punctuation.definition.tag.begin.html
//   ^^^^^^^^ entity.name.tag.template.html
//            ^^^^ entity.other.attribute-name.html
//                ^ punctuation.separator.key-value.html
//                       ^ punctuation.definition.tag.end.html

// <- text.haml.embedded.html
    </template>
//  ^^^^^^^^^^^ meta.tag - meta.tag meta.tag - text.haml
//  ^^ punctuation.definition.tag.begin.html
//    ^^^^^^^^ entity.name.tag.template.html
//            ^ punctuation.definition.tag.end.html

    <!--
    Jade Template Tests
    -->

    <template lang="jade"> foo </template>
//  ^^^^^^^^^^^^^^^^^^^^^^ meta.tag - source
//                        ^^^^^ text.jade.embedded.html - meta.tag
//                             ^^^^^^^^^^^ meta.tag - source

    <template lang="jade"> foo --> </template>
//  ^^^^^^^^^^^^^^^^^^^^^^ meta.tag - source
//                        ^^^^^^^^^ text.jade.embedded.html - meta.tag - comment
//                                 ^^^^^^^^^^^ meta.tag - source

    <template lang="jade"> <!-- foo </template>
//  ^^^^^^^^^^^^^^^^^^^^^^ meta.tag - source
//                        ^^^^^^^^^^ text.jade.embedded.html - meta.tag - comment
//                                  ^^^^^^^^^^^ meta.tag - source

    <template lang="jade"> <!-- foo --> </template>
//  ^^^^^^^^^^^^^^^^^^^^^^ meta.tag - source
//                        ^^^^^^^^^^^^^^ text.jade.embedded.html - meta.tag - comment
//                                      ^^^^^^^^^^^ meta.tag - source

    <template lang="jade">

// <- text.jade.embedded.html

    </template>
//  ^^^^^^^^^^^ meta.tag - meta.tag meta.tag - text.jade


    <template lang="jade">
//  ^^^^^^^^^^ meta.tag - meta.tag meta.tag - meta.attribute-with-value
//            ^^^^^^^^^^^ meta.tag meta.attribute-with-value.lang.html - meta.tag meta.tag
//                       ^ meta.tag.template.begin.html - meta.tag meta.tag
//  ^ punctuation.definition.tag.begin.html
//   ^^^^^^^^ entity.name.tag.template.html
//            ^^^^ entity.other.attribute-name.html
//                ^ punctuation.separator.key-value.html
//                       ^ punctuation.definition.tag.end.html

// <- text.jade.embedded.html
    </template>
//  ^^^^^^^^^^^ meta.tag - meta.tag meta.tag - text.jade
//  ^^ punctuation.definition.tag.begin.html
//    ^^^^^^^^ entity.name.tag.template.html
//            ^ punctuation.definition.tag.end.html

    <!--
    Pug Template Tests
    -->

    <template lang="pug">
//  ^^^^^^^^^^ meta.tag - meta.tag meta.tag - meta.attribute-with-value
//            ^^^^^^^^^^ meta.tag meta.attribute-with-value.lang.html - meta.tag meta.tag
//                      ^ meta.tag.template.begin.html - meta.tag meta.tag
//  ^ punctuation.definition.tag.begin.html
//   ^^^^^^^^ entity.name.tag.template.html
//            ^^^^ entity.other.attribute-name.html
//                ^ punctuation.separator.key-value.html
//                      ^ punctuation.definition.tag.end.html

// <- text.pug.embedded.html
    </template>
//  ^^^^^^^^^^^ meta.tag - meta.tag meta.tag - text.pug
//  ^^ punctuation.definition.tag.begin.html
//    ^^^^^^^^ entity.name.tag.template.html
//            ^ punctuation.definition.tag.end.html

    <!--
    Slim Template Tests
    -->

    <template lang="slm">
//  ^^^^^^^^^^ meta.tag - meta.tag meta.tag - meta.attribute-with-value
//            ^^^^^^^^^^ meta.tag meta.attribute-with-value.lang.html - meta.tag meta.tag
//                      ^ meta.tag.template.begin.html - meta.tag meta.tag
//  ^ punctuation.definition.tag.begin.html
//   ^^^^^^^^ entity.name.tag.template.html
//            ^^^^ entity.other.attribute-name.html
//                ^ punctuation.separator.key-value.html
//                      ^ punctuation.definition.tag.end.html

// <- text.slim.embedded.html
    </template>
//  ^^^^^^^^^^^ meta.tag - meta.tag meta.tag - text.slm
//  ^^ punctuation.definition.tag.begin.html
//    ^^^^^^^^ entity.name.tag.template.html
//            ^ punctuation.definition.tag.end.html
