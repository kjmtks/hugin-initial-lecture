# @Model.Lecture.Subject

@Model.Lecture.Description

<script language="activity" ref="python3.xml">
  <Name>python3/test1</Name>
  <Subject>Python</Subject>
  <Deadline>@ViewBag.deadline</Deadline>
  <Description>
print `Hello, World!!`
  </Description>
  <CodeAnswer>print("Hello, World!!")</CodeAnswer>
  <NumOfTestCases>1</NumOfTestCases>
  <TestCase1Answer>Hello, World!!</TestCase1Answer>
  <ConfirmAutomatically>true</ConfirmAutomatically>
  <CanSubmitBeforeRun>false</CanSubmitBeforeRun>
  <CanSubmitBeforeAccept>false</CanSubmitBeforeAccept>
  <CanValidateBeforeRun>false</CanValidateBeforeRun>
</script>

<script language="activity" ref="python3.xml">
  <Name>python3/test2</Name>
  <Subject>Draw Graph</Subject>
  <Deadline>@ViewBag.deadline</Deadline>
  <Description>
Draw a graph $ y = 1 - \exp\left(-x/20\right) $
  </Description>
  <Tags>ToBeGraded</Tags>
  <CodeDefault>
import numpy as np
import matplotlib.pyplot as plt
x = np.arange(0, 100, 0.1)
y = 1 - np.exp(-x / 20)
plt.plot(x, y)
plt.savefig('mygraph01.png')
  </CodeDefault>
  <NumOfCsvFiles>2</NumOfCsvFiles>
  <Csv1Name>data1.csv</Csv1Name>
  <Csv2Name>data2.csv</Csv2Name>
</script>

<script language="activity" ref="upload.xml">
  <Name>python3/test3</Name>
  <Subject>File Upload</Subject>
  <Deadline>@ViewBag.deadline</Deadline>
  <FileName>file.pdf</FileName>
  <AllowedContentTypes>application/pdf</AllowedContentTypes>
</script>

<script language="activity" ref="form.xml">
  <Name>python3/test4</Name>
  <Subject>Form</Subject>
  <Deadline>@ViewBag.deadline</Deadline>
  <Forms>

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

  </Forms>
</script>

