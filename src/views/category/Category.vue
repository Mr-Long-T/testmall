<template>
  <div class="wrapper">
    <ul class="content">
      <button @click="btnClick">按钮</button>
      <li>列表1</li>
      <li>列表2</li>
      <li>列表3</li>
      <li>列表4</li>
      <li>列表5</li>
      <li>列表6</li>
      <li>列表7</li>
      <li>列表8</li>
      <li>列表9</li>
      <li>列表10</li>
      <li>列表11</li>
      <li>列表12</li>
      <li>列表13</li>
      <li>列表14</li>
      <li>列表15</li>
      <li>列表16</li>
      <li>列表17</li>
      <li>列表18</li>
      <li>列表19</li>
      <li>列表20</li>
      <li>列表21</li>
      <li>列表22</li>
      <li>列表23</li>
      <li>列表24</li>
      <li>列表25</li>
      <li>列表26</li>
      <li>列表27</li>
      <li>列表28</li>
      <li>列表29</li>
      <li>列表30</li>
      <li>列表31</li>
      <li>列表32</li>
      <li>列表33</li>
      <li>列表34</li>
      <li>列表35</li>
      <li>列表36</li>
      <li>列表37</li>
      <li>列表38</li>
      <li>列表39</li>
      <li>列表40</li>
      <li>列表41</li>
      <li>列表42</li>
      <li>列表43</li>
      <li>列表44</li>
      <li>列表45</li>
      <li>列表46</li>
      <li>列表47</li>
      <li>列表48</li>
      <li>列表49</li>
      <li>列表50</li>
      <li>列表51</li>
      <li>列表52</li>
      <li>列表53</li>
      <li>列表54</li>
      <li>列表55</li>
      <li>列表56</li>
      <li>列表57</li>
      <li>列表58</li>
      <li>列表59</li>
      <li>列表60</li>
      <li>列表61</li>
      <li>列表62</li>
      <li>列表63</li>
      <li>列表64</li>
      <li>列表65</li>
      <li>列表66</li>
      <li>列表67</li>
      <li>列表68</li>
      <li>列表69</li>
      <li>列表70</li>
      <li>列表71</li>
      <li>列表72</li>
      <li>列表73</li>
      <li>列表74</li>
      <li>列表75</li>
      <li>列表76</li>
      <li>列表77</li>
      <li>列表78</li>
      <li>列表79</li>
      <li>列表80</li>
      <li>列表81</li>
      <li>列表82</li>
      <li>列表83</li>
      <li>列表84</li>
      <li>列表85</li>
      <li>列表86</li>
      <li>列表87</li>
      <li>列表88</li>
      <li>列表89</li>
      <li>列表90</li>
      <li>列表91</li>
      <li>列表92</li>
      <li>列表93</li>
      <li>列表94</li>
      <li>列表95</li>
      <li>列表96</li>
      <li>列表97</li>
      <li>列表98</li>
      <li>列表99</li>
      <li>列表100</li>
      <li>列表101</li>
      <li>列表102</li>
      <li>列表103</li>
      <li>列表104</li>
      <li>列表105</li>
      <li>列表106</li>
      <li>列表107</li>
      <li>列表108</li>
      <li>列表109</li>
      <li>列表110</li>
      <li>列表111</li>
      <li>列表112</li>
      <li>列表113</li>
      <li>列表114</li>
      <li>列表115</li>
      <li>列表116</li>
      <li>列表117</li>
      <li>列表118</li>
      <li>列表119</li>
      <li>列表120</li>
      <li>列表121</li>
      <li>列表122</li>
      <li>列表123</li>
      <li>列表124</li>
      <li>列表125</li>
      <li>列表126</li>
      <li>列表127</li>
      <li>列表128</li>
      <li>列表129</li>
      <li>列表130</li>
      <li>列表131</li>
      <li>列表132</li>
      <li>列表133</li>
      <li>列表134</li>
      <li>列表135</li>
      <li>列表136</li>
      <li>列表137</li>
      <li>列表138</li>
      <li>列表139</li>
      <li>列表140</li>
      <li>列表141</li>
      <li>列表142</li>
      <li>列表143</li>
      <li>列表144</li>
      <li>列表145</li>
      <li>列表146</li>
      <li>列表147</li>
      <li>列表148</li>
      <li>列表149</li>
      <li>列表150</li>
    </ul>
  </div>
</template>

<script>
import BScroll from 'better-scroll'

export default {
  name: "Category",
  data(){
    return {
      scroll: null
    }
  },
  //在created()中，不能拿到dom元素
  mounted() {
    this.scroll = new BScroll(document.querySelector('.wrapper'), {
      probeType: 3,  //监听滚动位置, 3表示只要是滚动就监听
      pullUpLoad: true,   //上拉加载更多
    })
    this.scroll.on('scroll' , (position) => {
      console.log(position);
    })
    this.scroll.on('pullingUp', () => {
      console.log('上拉加载更多');
    })
  },
  methods: {
    btnClick() {
      alert('btnClick')
    }
  }
}
</script>

<style scoped>
  .wrapper{
    height: 250px;
    background-color: #42b983;

    overflow: hidden;
    /*overflow-y: scroll;*/
  }
</style>
