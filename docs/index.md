# WaveDrom Markdown Syntax

## Signal Example

???+ note "Markdown"
    ```markdown
    wavedrom (
        { signal: [{ name: "Alfa", wave: "01.zx=ud.23.456789" }] }
    )
    ```

???+ example "Image"
    wavedrom (
        { signal: [{ name: "Alfa", wave: "01.zx=ud.23.456789" }] }
    )

## Schematic Example

???+ note "Markdown"
    ```markdown
    wavedrom (
        { assign: [
            ["out",
                ["|",
                    ["&", ["~", "a"], "b"],
                    ["&", ["~", "b"], "a"]
                ]
            ]
        ]}
    )
    ```

???+ example "Image"
    wavedrom (
        { assign: [
            ["out",
                ["|",
                    ["&", ["~", "a"], "b"],
                    ["&", ["~", "b"], "a"]
                ]
            ]
        ]}
    )

## Bit Field Example

???+ note "Markdown"
    ```markdown
    wavedrom (
        {reg: [
            {"bits": 7, "name": 51, "attr": "OP"},
            {"bits": 5, "name": "rd",     "attr": "dest"},
            {"bits": 3, "name": "funct3", "attr": ["ADD", "SLT", "SLTU", "AND", "OR", "XOR", "SLL", "SRL", "SUB", "SRA"]},
            {"bits": 5, "name": "rs1",    "attr": "src1"},
            {"bits": 5, "name": "rs2",    "attr": "src2"},
            {"bits": 7, "name": "funct7", "attr": [0, 0, 0, 0, 0, 0, 0, 0, 32, 32]}
        ]}
    )
    ```

???+ example "Image"
    wavedrom (
        {reg: [
            {"bits": 7, "name": 51, "attr": "OP"},
            {"bits": 5, "name": "rd",     "attr": "dest"},
            {"bits": 3, "name": "funct3", "attr": ["ADD", "SLT", "SLTU", "AND", "OR", "XOR", "SLL", "SRL", "SUB", "SRA"]},
            {"bits": 5, "name": "rs1",    "attr": "src1"},
            {"bits": 5, "name": "rs2",    "attr": "src2"},
            {"bits": 7, "name": "funct7", "attr": [0, 0, 0, 0, 0, 0, 0, 0, 32, 32]}
        ]}
    )
