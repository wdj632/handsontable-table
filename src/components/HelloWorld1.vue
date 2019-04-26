<template>
  <!--<hot-table :data="data" :rowHeaders="rowHeaders" :colHeaders="colHeaders" :readOnly="readOnly"></hot-table>-->
  <div>
    <HotTable :root="root" :settings="hotSettings"></HotTable>
  </div>
</template>

<script>
  import { HotTable } from '@handsontable/vue';

  export default {
    components: {
      HotTable
    },
    data: function() {
      return {
        root: 'test-hot',
        hotSettings: {
          data: [
            {
              "SellTotal": "0",
              "YKC": "51020",
              "bdQty": "0",
              "cgQty": "0",
              "cgthQty": "0",
              "ckname": "",
              "count": "30",
              "dcqty": "0",
              "drqty": "0",
              "id": "2019-04-30",
              "kcqty": "51020",
              "rl": "1",
              "thQty": "0",
              "xsQty": "0"
            },
            {
              "SellTotal": "0",
              "YKC": "51020",
              "bdQty": "0",
              "cgQty": "0",
              "cgthQty": "0",
              "ckname": "",
              "count": "30",
              "dcqty": "0",
              "drqty": "0",
              "id": "2019-04-29",
              "kcqty": "51020",
              "rl": "2",
              "thQty": "0",
              "xsQty": "0"
            },
            {
              "SellTotal": "0",
              "YKC": "51020",
              "bdQty": "0",
              "cgQty": "0",
              "cgthQty": "0",
              "ckname": "",
              "count": "30",
              "dcqty": "0",
              "drqty": "0",
              "id": "2019-04-28",
              "kcqty": "51020",
              "rl": "3",
              "thQty": "0",
              "xsQty": "0"
            },
            {
              "SellTotal": "0",
              "YKC": "51020",
              "bdQty": "0",
              "cgQty": "0",
              "cgthQty": "0",
              "ckname": "",
              "count": "30",
              "dcqty": "0",
              "drqty": "0",
              "id": "2019-04-27",
              "kcqty": "51020",
              "rl": "4",
              "thQty": "0",
              "xsQty": "0"
            },
            {
              "SellTotal": "0",
              "YKC": "51020",
              "bdQty": "0",
              "cgQty": "0",
              "cgthQty": "0",
              "ckname": "",
              "count": "30",
              "dcqty": "0",
              "drqty": "0",
              "id": "2019-04-26",
              "kcqty": "51020",
              "rl": "5",
              "thQty": "0",
              "xsQty": "0"
            },
            {
              "SellTotal": "0",
              "YKC": "51020",
              "bdQty": "0",
              "cgQty": "0",
              "cgthQty": "0",
              "ckname": "",
              "count": "30",
              "dcqty": "0",
              "drqty": "0",
              "id": "2019-04-25",
              "kcqty": "51020",
              "rl": "6",
              "thQty": "0",
              "xsQty": "0"
            },
            {
              "SellTotal": "0",
              "YKC": "51020",
              "bdQty": "0",
              "cgQty": "0",
              "cgthQty": "0",
              "ckname": "",
              "count": "30",
              "dcqty": "0",
              "drqty": "0",
              "id": "2019-04-24",
              "kcqty": "51020",
              "rl": "7",
              "thQty": "0",
              "xsQty": "0"
            },
            {
              "SellTotal": "0",
              "YKC": "51020",
              "bdQty": "0",
              "cgQty": "0",
              "cgthQty": "0",
              "ckname": "",
              "count": "30",
              "dcqty": "0",
              "drqty": "0",
              "id": "2019-04-23",
              "kcqty": "51020",
              "rl": "8",
              "thQty": "0",
              "xsQty": "0"
            },
            {
              "SellTotal": "88",
              "YKC": "51020",
              "bdQty": "0",
              "cgQty": "0",
              "cgthQty": "0",
              "ckname": "",
              "count": "30",
              "dcqty": "0",
              "drqty": "0",
              "id": "2019-04-22",
              "kcqty": "51019",
              "rl": "9",
              "thQty": "0",
              "xsQty": "1"
            },
            {
              "SellTotal": "0",
              "YKC": "51020",
              "bdQty": "0",
              "cgQty": "0",
              "cgthQty": "0",
              "ckname": "",
              "count": "30",
              "dcqty": "0",
              "drqty": "0",
              "id": "2019-04-21",
              "kcqty": "51019",
              "rl": "10",
              "thQty": "0",
              "xsQty": "0"
            },
            {
              "SellTotal": "0",
              "YKC": "51020",
              "bdQty": "0",
              "cgQty": "0",
              "cgthQty": "0",
              "ckname": "",
              "count": "30",
              "dcqty": "0",
              "drqty": "0",
              "id": "2019-04-20",
              "kcqty": "51019",
              "rl": "11",
              "thQty": "0",
              "xsQty": "0"
            },
            {
              "SellTotal": "0",
              "YKC": "51020",
              "bdQty": "0",
              "cgQty": "0",
              "cgthQty": "0",
              "ckname": "",
              "count": "30",
              "dcqty": "0",
              "drqty": "0",
              "id": "2019-04-19",
              "kcqty": "51019",
              "rl": "12",
              "thQty": "0",
              "xsQty": "0"
            },
            {
              "SellTotal": "458",
              "YKC": "51020",
              "bdQty": "0",
              "cgQty": "0",
              "cgthQty": "0",
              "ckname": "",
              "count": "30",
              "dcqty": "0",
              "drqty": "0",
              "id": "2019-04-18",
              "kcqty": "51017",
              "rl": "13",
              "thQty": "0",
              "xsQty": "2"
            },
            {
              "SellTotal": "0",
              "YKC": "51020",
              "bdQty": "0",
              "cgQty": "0",
              "cgthQty": "0",
              "ckname": "",
              "count": "30",
              "dcqty": "0",
              "drqty": "0",
              "id": "2019-04-17",
              "kcqty": "51017",
              "rl": "14",
              "thQty": "0",
              "xsQty": "0"
            },
            {
              "SellTotal": "0",
              "YKC": "51020",
              "bdQty": "0",
              "cgQty": "0",
              "cgthQty": "0",
              "ckname": "",
              "count": "30",
              "dcqty": "0",
              "drqty": "0",
              "id": "2019-04-16",
              "kcqty": "51017",
              "rl": "15",
              "thQty": "0",
              "xsQty": "0"
            },
            {
              "SellTotal": "0",
              "YKC": "51020",
              "bdQty": "0",
              "cgQty": "0",
              "cgthQty": "0",
              "ckname": "",
              "count": "30",
              "dcqty": "0",
              "drqty": "0",
              "id": "2019-04-15",
              "kcqty": "51017",
              "rl": "16",
              "thQty": "0",
              "xsQty": "0"
            },
            {
              "SellTotal": "0",
              "YKC": "51020",
              "bdQty": "0",
              "cgQty": "0",
              "cgthQty": "0",
              "ckname": "",
              "count": "30",
              "dcqty": "0",
              "drqty": "0",
              "id": "2019-04-14",
              "kcqty": "51017",
              "rl": "17",
              "thQty": "0",
              "xsQty": "0"
            },
            {
              "SellTotal": "0",
              "YKC": "51020",
              "bdQty": "0",
              "cgQty": "0",
              "cgthQty": "0",
              "ckname": "",
              "count": "30",
              "dcqty": "0",
              "drqty": "0",
              "id": "2019-04-13",
              "kcqty": "51017",
              "rl": "18",
              "thQty": "0",
              "xsQty": "0"
            },
            {
              "SellTotal": "0",
              "YKC": "51020",
              "bdQty": "0",
              "cgQty": "0",
              "cgthQty": "0",
              "ckname": "",
              "count": "30",
              "dcqty": "0",
              "drqty": "0",
              "id": "2019-04-12",
              "kcqty": "51017",
              "rl": "19",
              "thQty": "0",
              "xsQty": "0"
            },
            {
              "SellTotal": "0",
              "YKC": "51020",
              "bdQty": "0",
              "cgQty": "0",
              "cgthQty": "0",
              "ckname": "",
              "count": "30",
              "dcqty": "0",
              "drqty": "0",
              "id": "2019-04-11",
              "kcqty": "51017",
              "rl": "20",
              "thQty": "0",
              "xsQty": "0"
            },
            {
              "SellTotal": "0",
              "YKC": "51020",
              "bdQty": "0",
              "cgQty": "0",
              "cgthQty": "0",
              "ckname": "",
              "count": "30",
              "dcqty": "0",
              "drqty": "0",
              "id": "2019-04-10",
              "kcqty": "51017",
              "rl": "21",
              "thQty": "0",
              "xsQty": "0"
            },
            {
              "SellTotal": "0",
              "YKC": "51020",
              "bdQty": "0",
              "cgQty": "0",
              "cgthQty": "0",
              "ckname": "",
              "count": "30",
              "dcqty": "0",
              "drqty": "0",
              "id": "2019-04-09",
              "kcqty": "51017",
              "rl": "22",
              "thQty": "0",
              "xsQty": "0"
            },
            {
              "SellTotal": "210",
              "YKC": "51020",
              "bdQty": "0",
              "cgQty": "0",
              "cgthQty": "0",
              "ckname": "",
              "count": "30",
              "dcqty": "0",
              "drqty": "0",
              "id": "2019-04-08",
              "kcqty": "51016",
              "rl": "23",
              "thQty": "0",
              "xsQty": "1"
            },
            {
              "SellTotal": "0",
              "YKC": "51020",
              "bdQty": "0",
              "cgQty": "0",
              "cgthQty": "0",
              "ckname": "",
              "count": "30",
              "dcqty": "0",
              "drqty": "0",
              "id": "2019-04-07",
              "kcqty": "51016",
              "rl": "24",
              "thQty": "0",
              "xsQty": "0"
            },
            {
              "SellTotal": "0",
              "YKC": "51020",
              "bdQty": "0",
              "cgQty": "0",
              "cgthQty": "0",
              "ckname": "",
              "count": "30",
              "dcqty": "0",
              "drqty": "0",
              "id": "2019-04-06",
              "kcqty": "51016",
              "rl": "25",
              "thQty": "0",
              "xsQty": "0"
            },
            {
              "SellTotal": "0",
              "YKC": "51020",
              "bdQty": "0",
              "cgQty": "0",
              "cgthQty": "0",
              "ckname": "",
              "count": "30",
              "dcqty": "0",
              "drqty": "0",
              "id": "2019-04-05",
              "kcqty": "51016",
              "rl": "26",
              "thQty": "0",
              "xsQty": "0"
            },
            {
              "SellTotal": "0",
              "YKC": "51020",
              "bdQty": "0",
              "cgQty": "0",
              "cgthQty": "0",
              "ckname": "",
              "count": "30",
              "dcqty": "0",
              "drqty": "0",
              "id": "2019-04-04",
              "kcqty": "51016",
              "rl": "27",
              "thQty": "0",
              "xsQty": "0"
            },
            {
              "SellTotal": "0",
              "YKC": "51020",
              "bdQty": "0",
              "cgQty": "0",
              "cgthQty": "0",
              "ckname": "",
              "count": "30",
              "dcqty": "0",
              "drqty": "0",
              "id": "2019-04-03",
              "kcqty": "51016",
              "rl": "28",
              "thQty": "0",
              "xsQty": "0"
            },
            {
              "SellTotal": "248",
              "YKC": "51020",
              "bdQty": "0",
              "cgQty": "0",
              "cgthQty": "0",
              "ckname": "",
              "count": "30",
              "dcqty": "0",
              "drqty": "0",
              "id": "2019-04-02",
              "kcqty": "51015",
              "rl": "29",
              "thQty": "0",
              "xsQty": "1"
            },
            {
              "SellTotal": "0",
              "YKC": "51020",
              "bdQty": "0",
              "cgQty": "0",
              "cgthQty": "0",
              "ckname": "",
              "count": "30",
              "dcqty": "0",
              "drqty": "0",
              "id": "2019-04-01",
              "kcqty": "51015",
              "rl": "30",
              "thQty": "0",
              "xsQty": "0"
            }
          ],       //数据，可以是数据，对象
          startRows: 11,//行列范围
          startCols: 6,
          minRows: 5,  //最小行列
          minCols: 5,
          maxRows: 20,  //最大行列
          maxCols: 20,
          rowHeaders: false,//列表头
          colHeaders:   [
            '序号', '时间', '销售金额', '销售数量', '调出数量','调入数量','调出调入仓库','其他变动数量','采购数量','库存数量'
          ],//自定义列表头or 布尔值
          // minSpareCols: 2, //列留白
          // minSpareRows: 2,//行留白
          currentRowClassName: 'currentRow', //为选中行添加类名，可以更改样式
          currentColClassName: 'currentCol',//为选中列添加类名
          autoWrapRow: false, //自动换行

          contextMenu: {   //自定义右键菜单，可汉化，默认布尔值
            items: {
              "row_above": {
                name:'上方插入一行'
              },
              "row_below": {
                name:'下方插入一行'
              },
              "col_left": {
                name:'左方插入列'
              },
              "col_right": {
                name:'右方插入列'
              },
              "hsep1": "---------", //提供分隔线
              "remove_row": {
                name: '删除行',
              },
              "remove_col": {
                name: '删除列',
              },
              "make_read_only": {
                name: '只读',
              },
              "borders": {
                name: '表格线',
              },
              "commentsAddEdit": {
                name: '添加备注',
              },
              "commentsRemove": {
                name: '取消备注',
              },
              "freeze_column": {
                name: '固定列',
              },
              "unfreeze_column": {
                name: '取消列固定',
              },
              "hsep2": "---------",
            }
          },//右键效果
          fillHandle: true, //选中拖拽复制 possible values: true, false, "horizontal", "vertical"
          fixedColumnsLeft: 0,//固定左边列数
          fixedRowsTop: 0,//固定上边列数
          // mergeCells: [   //合并
          //   {row: 1, col: 1, rowspan: 3, colspan: 3},  //指定合并，从（1,1）开始行3列3合并成一格
          //   {row: 3, col: 4, rowspan: 2, colspan: 2}
          // ],
          readOnly: true,
          filters: true,
          dropdownMenu: true,
          columns: [     //添加每一列的数据类型和一些配置
            {data: 'rl'},
            {
              data: 'id',
            },
            {data: 'SellTotal'},
            {data: 'xsQty'},
            {data: 'dcqty'},
            {data: 'drqty'},
            {data: 'ckname'},
            {data: 'bdQty'},
            {data: 'cgthQty'},
            {data: 'kcqty'},
          ],
          manualColumnFreeze: true, //手动固定列
          manualColumnMove: true, //手动移动列
          manualRowMove: true,   //手动移动行
          manualColumnResize: true,//手工更改列距
          manualRowResize: true,//手动更改行距
          comments: false, //添加注释
          width: 880,
          height: 487,
          // fixedRowsBottom: 2,//固定下面两行
          cell: [
            {row: 1, col: 1, comment: {value: 'this is test'}}, //注释
          ],
          language: 'zh-CN',
          customBorders:[],//添加边框
          columnSorting: true,//排序
          stretchH: 'all',//根据宽度横向扩展，last:只扩展最后一列，none：默认不扩展
        },
      };
    },

    mounted(){

    },
  }
</script>

<style src="../../node_modules/handsontable/dist/handsontable.full.css"></style>
