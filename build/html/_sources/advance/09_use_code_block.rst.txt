.. _topics-09_use_code_block:

====
代码块
====

c++代码样例
====

.. code-block:: c++

    #include <stdio.h>
    
    int main(int argc, char* argv[]) {
        printf("HelloWorld!);
        return 0;
    }

bash代码样例
====

.. code-block:: bash

    #!/bin/sh
    #================================================
    #FileName   : test.sh
    #Author     : wzx
    #Description:
    #DateTime   : 2019-05-02 11:00:00
    #Version    : V1.0
    #Other      :
    #================================================

    for opt in "${@}"; do
    case $opt in
        --input-model=*)
        export input_model="$(echo "$opt" | cut -d '=' -f 2-)"
        ;;
        --input-picture=*)
        export input_picture="$(echo "$opt" | cut -d '=' -f 2-)"
        ;;
        --help)
        echo ${USAGE_LINE}
        exit
        ;;
        *)
        echo ${USAGE_LINE}
        exit
        ;;
    esac
    done

python代码样例
====

.. code-block:: python

    try:
        f = open('/path/to/file', 'r')
        print(f.read())
    finally:
        if f:
            f.close()

    with open('/path/to/file', 'r') as f:
        print(f.read())

    f = open('/Users/michael/gbk.txt', 'r', encoding='gbk', errors='ignore')

json对象样例展示
====

.. code-block:: json

    {
        "name": "BeJson",
        "url": "http://www.bejson.com",
        "page": 88,
        "isNonProfit": true,
        "address": {
            "street": "科技园路.",
            "city": "江苏苏州",
            "country": "中国"
        },
        "links": [
            {
                "name": "Google",
                "url": "http://www.google.com"
            },
            {
                "name": "Baidu",
                "url": "http://www.baidu.com"
            },
            {
                "name": "SoSo",
                "url": "http://www.SoSo.com"
            }
        ]
    }