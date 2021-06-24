# {{ lecture.subject }}

{{ lecture.description }}

<script language="activity" ref="python3.xml">
  <name>python3/test1</name>
  <subject>Python</subject>
  <deadline>{{ deadline }}</deadline>
  <description>
print `Hello, World!!`
  </description>
  <code_answer>print("Hello, World!!")</code_answer>
  <num_of_testcases>1</num_of_testcases>
  <testcase1answer>Hello, World!!</testcase1answer>
  <confirm_automatically>true</confirm_automatically>
  <can_submit_before_run>false</can_submit_before_run>
  <can_submit_before_accept>false</can_submit_before_accept>
  <can_validate_before_run>false</can_validate_before_run>
</script>

<script language="activity" ref="blockly-basic.xml">
  <name>blockly/test1</name>
  <subject>Blockly</subject>
  <deadline>{{ deadline }}</deadline>
  <description>
print `Hello, World!!` 10 times
  </description>
  <default>
<xml xmlns="https://developers.google.com/blockly/xml"><block type="controls_repeat" id="m,CEp}{}IjQ*0NJkJ.%f" x="333" y="135"><field name="TIMES">0</field><statement name="DO"><block type="text_print" id="OV986kJ%kP4r@D$$=ybY"><value name="TEXT"><block type="text" id="7B-ZH5|~ir7]{#D5xiv{"><field name="TEXT"></field></block></value></block></statement></block></xml>
  </default>
  <height>800px</height>
  <num_of_testcases>1</num_of_testcases>
  <testcase1answer>Hello, World!!
Hello, World!!
Hello, World!!
Hello, World!!
Hello, World!!
Hello, World!!
Hello, World!!
Hello, World!!
Hello, World!!
Hello, World!!</testcase1answer>
  <confirm_automatically>true</confirm_automatically>
  <can_submit_before_run>false</can_submit_before_run>
  <can_submit_before_accept>false</can_submit_before_accept>
  <can_validate_before_run>false</can_validate_before_run>
</script>

<script language="activity" ref="python3.xml">
  <name>python3/test2</name>
  <subject>Draw Graph</subject>
  <deadline>{{ deadline }}</deadline>
  <description>
Draw a graph $ y = 1 - \exp\left(-x/20\right) $
  </description>
  <tags>ToBeGraded</tags>
  <code_default>
import numpy as np
import matplotlib.pyplot as plt
x = np.arange(0, 100, 0.1)
y = 1 - np.exp(-x / 20)
plt.plot(x, y)
plt.savefig('mygraph01.png')
  </code_default>
  <num_of_csv_files>2</num_of_csv_files>
  <csv1name>data1.csv</csv1name>
  <csv2name>data2.csv</csv2name>
</script>

<script language="activity" ref="upload.xml">
  <name>python3/test3</name>
  <subject>File Upload</subject>
  <deadline>{{ deadline }}</deadline>
  <file_name>file.pdf</file_name>
  <allowed_content_types>application/pdf</allowed_content_types>
</script>

<script language="activity" ref="form.xml">
  <name>python3/test4</name>
  <subject>Form</subject>
  <deadline>@ViewBag.deadline</deadline>
  <forms>

      <Text>TEXT</Text>

      <Select Name="select1" Label="SELECT" >
        <Option Value="1" Answer="true">One</Option>
        <Option Value="2" Default="true">Two</Option>
        <Option Value="3">Three</Option>
      </Select>

      <Radio Name="radio1" Label="RADIO" Block="true">
        <Option Value="1" Answer="true">One</Option>
        <Option Value="2" Default="true">Two</Option>
        <Option Value="3">Three</Option>
      </Radio>

      <Checkbox Name="chk1" True="On" False="Off" Default="true" Answer="true">CHECKBOX</Checkbox>

      <String Name="str1" Label="STRING" Size="small">
        <Default>???</Default>
        <Answer>AAA</Answer>           
      </String>

      <Textarea Name="textarea1" Label="TEXTAREA" Rows="6">
       <Default>Hello</Default>
       <Answer>Hello</Answer>
      </Textarea>

  </forms>
</script>

