<template>
    <div class="layout">
        <Layout>
            <Header>
                <Menu mode="horizontal" theme="dark" active-name="1">
                    <div class="layout-logo layout-name">客户管理系统</div>
                    <div class="layout-nav">
                        <menu-item name="1">
                            <Icon type="ios-navigate"></Icon>
                            Item 1
                        </menu-item>
                        <menu-item name="2">
                            <Icon type="ios-keypad"></Icon>
                            Item 2
                        </menu-item>
                        <menu-item name="3">
                            <Icon type="ios-analytics"></Icon>
                            Item 3
                        </menu-item>
                        <menu-item name="4">
                            <Icon type="ios-paper"></Icon>
                            Item 4
                        </menu-item>
                    </div>
                </Menu>
            </Header>
            <Layout>
                <Sider hide-trigger :style="{background: '#fff'}">
                    <Menu active-name="1-2" theme="light" width="auto" :open-names="['1']">
                        <Submenu name="1">
                            <template slot="title">
                                <Icon type="ios-navigate"></Icon>
                                Item 1
                            </template>
                            <menu-item name="1-1">Option 1</menu-item>
                            <menu-item name="1-2">Option 2</menu-item>
                            <menu-item name="1-3">Option 3</menu-item>
                        </Submenu>
                        <Submenu name="2">
                            <template slot="title">
                                <Icon type="ios-keypad"></Icon>
                                Item 2
                            </template>
                            <menu-item name="2-1">Option 1</menu-item>
                            <menu-item name="2-2">Option 2</menu-item>
                        </Submenu>
                        <Submenu name="3">
                            <template slot="title">
                                <Icon type="ios-analytics"></Icon>
                                Item 3
                            </template>
                            <menu-item name="3-1">Option 1</menu-item>
                            <menu-item name="3-2">Option 2</menu-item>
                        </Submenu>
                    </Menu>
                </Sider>
                <Layout :style="{padding: '0 24px 24px'}">
                    <Breadcrumb :style="{margin: '24px 0'}">
                        <BreadcrumbItem>Home</BreadcrumbItem>
                        <BreadcrumbItem>Components</BreadcrumbItem>
                        <BreadcrumbItem>Layout</BreadcrumbItem>
                    </Breadcrumb>
                    <Content :style="{padding: '24px', minHeight: '280px', background: '#fff'}">
                        Content
                    </Content>
                </Layout>
            </Layout>
        </Layout>
    </div>
</template>
<script>
export default {
  name: 'Home',
  data () {
    return {
    }
  }
}
</script>
<style less  scoped>
.layout{
    border: 1px solid #d7dde4;
    background: #f5f7f9;
    position: relative;
    border-radius: 4px;
    overflow: auto;
    height: 100%;
}
.ivu-layout{
    height: 100%;
}
.layout-logo{
    float: left;
    position: relative;
    top: 0;
    left: 20px;
}
.layout-name{
    color: white;
    text-align: left;
    font-size: 18px;
}
.layout-nav{
    width: 420px;
    margin: 0 auto;
    margin-right: 20px;
}
</style>
