<template>
  <!--<hot-table :data="data" :rowHeaders="rowHeaders" :colHeaders="colHeaders" :readOnly="readOnly"></hot-table>-->
  <div>
    <!--<HotTable :root="root" :settings="hotSettings"></HotTable>-->
    <div id="hot"></div>
  </div>
</template>

<script>
  // import { HotTable } from '@handsontable/vue';
  var dataObject = [
    {
      id: 1,
      flag: 'EUR',
      currencyCode: 'EUR',
      currency: 'Euro',
      level: 0.9033,
      units: 'EUR / USD',
      asOf: '08/19/2019',
      onedChng: 0.0026
    },
    {
      id: 2,
      flag: 'JPY',
      currencyCode: 'JPY',
      currency: 'Japanese Yen',
      level: 124.3870,
      units: 'JPY / USD',
      asOf: '08/19/2019',
      onedChng: 0.0001
    },
    {
      id: 3,
      flag: 'GBP',
      currencyCode: 'GBP',
      currency: 'Pound Sterling',
      level: 0.6396,
      units: 'GBP / USD',
      asOf: '08/19/2019',
      onedChng: 0.00
    },
    {
      id: 4,
      flag: 'CHF',
      currencyCode: 'CHF',
      currency: 'Swiss Franc',
      level: 0.9775,
      units: 'CHF / USD',
      asOf: '08/19/2019',
      onedChng: 0.0008
    },
    {
      id: 5,
      flag: 'CAD',
      currencyCode: 'CAD',
      currency: 'Canadian Dollar',
      level: 1.3097,
      units: 'CAD / USD',
      asOf: '08/19/2019',
      onedChng: -0.0005
    },
    {
      id: 6,
      flag: 'AUD',
      currencyCode: 'AUD',
      currency: 'Australian Dollar',
      level: 1.3589,
      units: 'AUD / USD',
      asOf: '08/19/2019',
      onedChng: 0.0020
    },
    {
      id: 7,
      flag: 'NZD',
      currencyCode: 'NZD',
      currency: 'New Zealand Dollar',
      level: 1.5218,
      units: 'NZD / USD',
      asOf: '08/19/2019',
      onedChng: -0.0036
    },
    {
      id: 8,
      flag: 'SEK',
      currencyCode: 'SEK',
      currency: 'Swedish Krona',
      level: 8.5280,
      units: 'SEK / USD',
      asOf: '08/19/2019',
      onedChng: 0.0016
    },
    {
      id: 9,
      flag: 'NOK',
      currencyCode: 'NOK',
      currency: 'Norwegian Krone',
      level: 8.2433,
      units: 'NOK / USD',
      asOf: '08/19/2019',
      onedChng: 0.0008
    },
    {
      id: 10,
      flag: 'BRL',
      currencyCode: 'BRL',
      currency: 'Brazilian Real',
      level: 3.4806,
      units: 'BRL / USD',
      asOf: '08/19/2019',
      onedChng: -0.0009
    },
    {
      id: 11,
      flag: 'CNY',
      currencyCode: 'CNY',
      currency: 'Chinese Yuan',
      level: 6.3961,
      units: 'CNY / USD',
      asOf: '08/19/2019',
      onedChng: 0.0004
    },
    {
      id: 12,
      flag: 'RUB',
      currencyCode: 'RUB',
      currency: 'Russian Rouble',
      level: 65.5980,
      units: 'RUB / USD',
      asOf: '08/19/2019',
      onedChng: 0.0059
    },
    {
      id: 13,
      flag: 'INR',
      currencyCode: 'INR',
      currency: 'Indian Rupee',
      level: 65.3724,
      units: 'INR / USD',
      asOf: '08/19/2019',
      onedChng: 0.0026
    },
    {
      id: 14,
      flag: 'TRY',
      currencyCode: 'TRY',
      currency: 'New Turkish Lira',
      level: 2.8689,
      units: 'TRY / USD',
      asOf: '08/19/2019',
      onedChng: 0.0092
    },
    {
      id: 15,
      flag: 'THB',
      currencyCode: 'THB',
      currency: 'Thai Baht',
      level: 35.5029,
      units: 'THB / USD',
      asOf: '08/19/2019',
      onedChng: 0.0044
    },
    {
      id: 16,
      flag: 'IDR',
      currencyCode: 'IDR',
      currency: 'Indonesian Rupiah',
      level: 13.83,
      units: 'IDR / USD',
      asOf: '08/19/2019',
      onedChng: -0.0009
    },
    {
      id: 17,
      flag: 'MYR',
      currencyCode: 'MYR',
      currency: 'Malaysian Ringgit',
      level: 4.0949,
      units: 'MYR / USD',
      asOf: '08/19/2019',
      onedChng: 0.0010
    },
    {
      id: 18,
      flag: 'MXN',
      currencyCode: 'MXN',
      currency: 'Mexican New Peso',
      level: 16.4309,
      units: 'MXN / USD',
      asOf: '08/19/2019',
      onedChng: 0.0017
    },
    {
      id: 19,
      flag: 'ARS',
      currencyCode: 'ARS',
      currency: 'Argentinian Peso',
      level: 9.2534,
      units: 'ARS / USD',
      asOf: '08/19/2019',
      onedChng: 0.0011
    },
    {
      id: 20,
      flag: 'DKK',
      currencyCode: 'DKK',
      currency: 'Danish Krone',
      level: 6.7417,
      units: 'DKK / USD',
      asOf: '08/19/2019',
      onedChng: 0.0025
    },
    {
      id: 21,
      flag: 'ILS',
      currencyCode: 'ILS',
      currency: 'Israeli New Sheqel',
      level: 3.8262,
      units: 'ILS / USD',
      asOf: '08/19/2019',
      onedChng: 0.0084
    },
    {
      id: 22,
      flag: 'PHP',
      currencyCode: 'PHP',
      currency: 'Philippine Peso',
      level: 46.3108,
      units: 'PHP / USD',
      asOf: '08/19/2019',
      onedChng: 0.0012
    }
  ];
  var currencyCodes = ['EUR', 'JPY', 'GBP', 'CHF', 'CAD', 'AUD', 'NZD', 'SEK', 'NOK', 'BRL', 'CNY', 'RUB', 'INR', 'TRY', 'THB', 'IDR', 'MYR', 'MXN', 'ARS', 'DKK', 'ILS', 'PHP'];
  var flagRenderer = function (instance, td, row, col, prop, value, cellProperties) {
    var currencyCode = value;
    while (td.firstChild) {
      td.removeChild(td.firstChild);
    }
    if (currencyCodes.indexOf(currencyCode) > -1) {
      var flagElement = document.createElement('DIV');
      flagElement.className = 'flag ' + currencyCode.toLowerCase();
      td.appendChild(flagElement);
    } else {
      var textNode = document.createTextNode(value === null ? '' : value);

      td.appendChild(textNode);
    }
  };
  var hotElement = document.querySelector('#hot');
  var hotElementContainer = hotElement.parentNode;
  var hotSettings = {
    data: dataObject,
    columns: [
      {
        data: 'id',
        type: 'numeric',
        width: 40
      },
      {
        data: 'flag',
        renderer: flagRenderer
      },
      {
        data: 'currencyCode',
        type: 'text'
      },
      {
        data: 'currency',
        type: 'text'
      },
      {
        data: 'level',
        type: 'numeric',
        numericFormat: {
          pattern: '0.0000'
        }
      },
      {
        data: 'units',
        type: 'text'
      },
      {
        data: 'asOf',
        type: 'date',
        dateFormat: 'MM/DD/YYYY'
      },
      {
        data: 'onedChng',
        type: 'numeric',
        numericFormat: {
          pattern: '0.00%'
        }
      }
    ],
    stretchH: 'all',
    width: 880,
    autoWrapRow: true,
    height: 487,
    maxRows: 22,
    manualRowResize: true,
    manualColumnResize: true,
    rowHeaders: true,
    colHeaders: [
      'ID',
      'Country',
      'Code',
      'Currency',
      'Level',
      'Units',
      'Date',
      'Change'
    ],
    manualRowMove: true,
    manualColumnMove: true,
    contextMenu: true,
    filters: true,
    dropdownMenu: true
  };
  var hot = new Handsontable(hotElement, hotSettings);
  export default {
    // components: {
    //   HotTable
    // },
    data: function() {
      // return {
      //   root: 'test-hot',
      //   hotSettings: {
      //     data: [
      //       {
      //         "SellTotal": "0",
      //         "YKC": "51020",
      //         "bdQty": "0",
      //         "cgQty": "0",
      //         "cgthQty": "0",
      //         "ckname": "",
      //         "count": "30",
      //         "dcqty": "0",
      //         "drqty": "0",
      //         "id": "2019-04-30",
      //         "kcqty": "51020",
      //         "rl": "1",
      //         "thQty": "0",
      //         "xsQty": "0"
      //       },
      //       {
      //         "SellTotal": "0",
      //         "YKC": "51020",
      //         "bdQty": "0",
      //         "cgQty": "0",
      //         "cgthQty": "0",
      //         "ckname": "",
      //         "count": "30",
      //         "dcqty": "0",
      //         "drqty": "0",
      //         "id": "2019-04-29",
      //         "kcqty": "51020",
      //         "rl": "2",
      //         "thQty": "0",
      //         "xsQty": "0"
      //       },
      //       {
      //         "SellTotal": "0",
      //         "YKC": "51020",
      //         "bdQty": "0",
      //         "cgQty": "0",
      //         "cgthQty": "0",
      //         "ckname": "",
      //         "count": "30",
      //         "dcqty": "0",
      //         "drqty": "0",
      //         "id": "2019-04-28",
      //         "kcqty": "51020",
      //         "rl": "3",
      //         "thQty": "0",
      //         "xsQty": "0"
      //       },
      //       {
      //         "SellTotal": "0",
      //         "YKC": "51020",
      //         "bdQty": "0",
      //         "cgQty": "0",
      //         "cgthQty": "0",
      //         "ckname": "",
      //         "count": "30",
      //         "dcqty": "0",
      //         "drqty": "0",
      //         "id": "2019-04-27",
      //         "kcqty": "51020",
      //         "rl": "4",
      //         "thQty": "0",
      //         "xsQty": "0"
      //       },
      //       {
      //         "SellTotal": "0",
      //         "YKC": "51020",
      //         "bdQty": "0",
      //         "cgQty": "0",
      //         "cgthQty": "0",
      //         "ckname": "",
      //         "count": "30",
      //         "dcqty": "0",
      //         "drqty": "0",
      //         "id": "2019-04-26",
      //         "kcqty": "51020",
      //         "rl": "5",
      //         "thQty": "0",
      //         "xsQty": "0"
      //       },
      //       {
      //         "SellTotal": "0",
      //         "YKC": "51020",
      //         "bdQty": "0",
      //         "cgQty": "0",
      //         "cgthQty": "0",
      //         "ckname": "",
      //         "count": "30",
      //         "dcqty": "0",
      //         "drqty": "0",
      //         "id": "2019-04-25",
      //         "kcqty": "51020",
      //         "rl": "6",
      //         "thQty": "0",
      //         "xsQty": "0"
      //       },
      //       {
      //         "SellTotal": "0",
      //         "YKC": "51020",
      //         "bdQty": "0",
      //         "cgQty": "0",
      //         "cgthQty": "0",
      //         "ckname": "",
      //         "count": "30",
      //         "dcqty": "0",
      //         "drqty": "0",
      //         "id": "2019-04-24",
      //         "kcqty": "51020",
      //         "rl": "7",
      //         "thQty": "0",
      //         "xsQty": "0"
      //       },
      //       {
      //         "SellTotal": "0",
      //         "YKC": "51020",
      //         "bdQty": "0",
      //         "cgQty": "0",
      //         "cgthQty": "0",
      //         "ckname": "",
      //         "count": "30",
      //         "dcqty": "0",
      //         "drqty": "0",
      //         "id": "2019-04-23",
      //         "kcqty": "51020",
      //         "rl": "8",
      //         "thQty": "0",
      //         "xsQty": "0"
      //       },
      //       {
      //         "SellTotal": "88",
      //         "YKC": "51020",
      //         "bdQty": "0",
      //         "cgQty": "0",
      //         "cgthQty": "0",
      //         "ckname": "",
      //         "count": "30",
      //         "dcqty": "0",
      //         "drqty": "0",
      //         "id": "2019-04-22",
      //         "kcqty": "51019",
      //         "rl": "9",
      //         "thQty": "0",
      //         "xsQty": "1"
      //       },
      //       {
      //         "SellTotal": "0",
      //         "YKC": "51020",
      //         "bdQty": "0",
      //         "cgQty": "0",
      //         "cgthQty": "0",
      //         "ckname": "",
      //         "count": "30",
      //         "dcqty": "0",
      //         "drqty": "0",
      //         "id": "2019-04-21",
      //         "kcqty": "51019",
      //         "rl": "10",
      //         "thQty": "0",
      //         "xsQty": "0"
      //       },
      //       {
      //         "SellTotal": "0",
      //         "YKC": "51020",
      //         "bdQty": "0",
      //         "cgQty": "0",
      //         "cgthQty": "0",
      //         "ckname": "",
      //         "count": "30",
      //         "dcqty": "0",
      //         "drqty": "0",
      //         "id": "2019-04-20",
      //         "kcqty": "51019",
      //         "rl": "11",
      //         "thQty": "0",
      //         "xsQty": "0"
      //       },
      //       {
      //         "SellTotal": "0",
      //         "YKC": "51020",
      //         "bdQty": "0",
      //         "cgQty": "0",
      //         "cgthQty": "0",
      //         "ckname": "",
      //         "count": "30",
      //         "dcqty": "0",
      //         "drqty": "0",
      //         "id": "2019-04-19",
      //         "kcqty": "51019",
      //         "rl": "12",
      //         "thQty": "0",
      //         "xsQty": "0"
      //       },
      //       {
      //         "SellTotal": "458",
      //         "YKC": "51020",
      //         "bdQty": "0",
      //         "cgQty": "0",
      //         "cgthQty": "0",
      //         "ckname": "",
      //         "count": "30",
      //         "dcqty": "0",
      //         "drqty": "0",
      //         "id": "2019-04-18",
      //         "kcqty": "51017",
      //         "rl": "13",
      //         "thQty": "0",
      //         "xsQty": "2"
      //       },
      //       {
      //         "SellTotal": "0",
      //         "YKC": "51020",
      //         "bdQty": "0",
      //         "cgQty": "0",
      //         "cgthQty": "0",
      //         "ckname": "",
      //         "count": "30",
      //         "dcqty": "0",
      //         "drqty": "0",
      //         "id": "2019-04-17",
      //         "kcqty": "51017",
      //         "rl": "14",
      //         "thQty": "0",
      //         "xsQty": "0"
      //       },
      //       {
      //         "SellTotal": "0",
      //         "YKC": "51020",
      //         "bdQty": "0",
      //         "cgQty": "0",
      //         "cgthQty": "0",
      //         "ckname": "",
      //         "count": "30",
      //         "dcqty": "0",
      //         "drqty": "0",
      //         "id": "2019-04-16",
      //         "kcqty": "51017",
      //         "rl": "15",
      //         "thQty": "0",
      //         "xsQty": "0"
      //       },
      //       {
      //         "SellTotal": "0",
      //         "YKC": "51020",
      //         "bdQty": "0",
      //         "cgQty": "0",
      //         "cgthQty": "0",
      //         "ckname": "",
      //         "count": "30",
      //         "dcqty": "0",
      //         "drqty": "0",
      //         "id": "2019-04-15",
      //         "kcqty": "51017",
      //         "rl": "16",
      //         "thQty": "0",
      //         "xsQty": "0"
      //       },
      //       {
      //         "SellTotal": "0",
      //         "YKC": "51020",
      //         "bdQty": "0",
      //         "cgQty": "0",
      //         "cgthQty": "0",
      //         "ckname": "",
      //         "count": "30",
      //         "dcqty": "0",
      //         "drqty": "0",
      //         "id": "2019-04-14",
      //         "kcqty": "51017",
      //         "rl": "17",
      //         "thQty": "0",
      //         "xsQty": "0"
      //       },
      //       {
      //         "SellTotal": "0",
      //         "YKC": "51020",
      //         "bdQty": "0",
      //         "cgQty": "0",
      //         "cgthQty": "0",
      //         "ckname": "",
      //         "count": "30",
      //         "dcqty": "0",
      //         "drqty": "0",
      //         "id": "2019-04-13",
      //         "kcqty": "51017",
      //         "rl": "18",
      //         "thQty": "0",
      //         "xsQty": "0"
      //       },
      //       {
      //         "SellTotal": "0",
      //         "YKC": "51020",
      //         "bdQty": "0",
      //         "cgQty": "0",
      //         "cgthQty": "0",
      //         "ckname": "",
      //         "count": "30",
      //         "dcqty": "0",
      //         "drqty": "0",
      //         "id": "2019-04-12",
      //         "kcqty": "51017",
      //         "rl": "19",
      //         "thQty": "0",
      //         "xsQty": "0"
      //       },
      //       {
      //         "SellTotal": "0",
      //         "YKC": "51020",
      //         "bdQty": "0",
      //         "cgQty": "0",
      //         "cgthQty": "0",
      //         "ckname": "",
      //         "count": "30",
      //         "dcqty": "0",
      //         "drqty": "0",
      //         "id": "2019-04-11",
      //         "kcqty": "51017",
      //         "rl": "20",
      //         "thQty": "0",
      //         "xsQty": "0"
      //       },
      //       {
      //         "SellTotal": "0",
      //         "YKC": "51020",
      //         "bdQty": "0",
      //         "cgQty": "0",
      //         "cgthQty": "0",
      //         "ckname": "",
      //         "count": "30",
      //         "dcqty": "0",
      //         "drqty": "0",
      //         "id": "2019-04-10",
      //         "kcqty": "51017",
      //         "rl": "21",
      //         "thQty": "0",
      //         "xsQty": "0"
      //       },
      //       {
      //         "SellTotal": "0",
      //         "YKC": "51020",
      //         "bdQty": "0",
      //         "cgQty": "0",
      //         "cgthQty": "0",
      //         "ckname": "",
      //         "count": "30",
      //         "dcqty": "0",
      //         "drqty": "0",
      //         "id": "2019-04-09",
      //         "kcqty": "51017",
      //         "rl": "22",
      //         "thQty": "0",
      //         "xsQty": "0"
      //       },
      //       {
      //         "SellTotal": "210",
      //         "YKC": "51020",
      //         "bdQty": "0",
      //         "cgQty": "0",
      //         "cgthQty": "0",
      //         "ckname": "",
      //         "count": "30",
      //         "dcqty": "0",
      //         "drqty": "0",
      //         "id": "2019-04-08",
      //         "kcqty": "51016",
      //         "rl": "23",
      //         "thQty": "0",
      //         "xsQty": "1"
      //       },
      //       {
      //         "SellTotal": "0",
      //         "YKC": "51020",
      //         "bdQty": "0",
      //         "cgQty": "0",
      //         "cgthQty": "0",
      //         "ckname": "",
      //         "count": "30",
      //         "dcqty": "0",
      //         "drqty": "0",
      //         "id": "2019-04-07",
      //         "kcqty": "51016",
      //         "rl": "24",
      //         "thQty": "0",
      //         "xsQty": "0"
      //       },
      //       {
      //         "SellTotal": "0",
      //         "YKC": "51020",
      //         "bdQty": "0",
      //         "cgQty": "0",
      //         "cgthQty": "0",
      //         "ckname": "",
      //         "count": "30",
      //         "dcqty": "0",
      //         "drqty": "0",
      //         "id": "2019-04-06",
      //         "kcqty": "51016",
      //         "rl": "25",
      //         "thQty": "0",
      //         "xsQty": "0"
      //       },
      //       {
      //         "SellTotal": "0",
      //         "YKC": "51020",
      //         "bdQty": "0",
      //         "cgQty": "0",
      //         "cgthQty": "0",
      //         "ckname": "",
      //         "count": "30",
      //         "dcqty": "0",
      //         "drqty": "0",
      //         "id": "2019-04-05",
      //         "kcqty": "51016",
      //         "rl": "26",
      //         "thQty": "0",
      //         "xsQty": "0"
      //       },
      //       {
      //         "SellTotal": "0",
      //         "YKC": "51020",
      //         "bdQty": "0",
      //         "cgQty": "0",
      //         "cgthQty": "0",
      //         "ckname": "",
      //         "count": "30",
      //         "dcqty": "0",
      //         "drqty": "0",
      //         "id": "2019-04-04",
      //         "kcqty": "51016",
      //         "rl": "27",
      //         "thQty": "0",
      //         "xsQty": "0"
      //       },
      //       {
      //         "SellTotal": "0",
      //         "YKC": "51020",
      //         "bdQty": "0",
      //         "cgQty": "0",
      //         "cgthQty": "0",
      //         "ckname": "",
      //         "count": "30",
      //         "dcqty": "0",
      //         "drqty": "0",
      //         "id": "2019-04-03",
      //         "kcqty": "51016",
      //         "rl": "28",
      //         "thQty": "0",
      //         "xsQty": "0"
      //       },
      //       {
      //         "SellTotal": "248",
      //         "YKC": "51020",
      //         "bdQty": "0",
      //         "cgQty": "0",
      //         "cgthQty": "0",
      //         "ckname": "",
      //         "count": "30",
      //         "dcqty": "0",
      //         "drqty": "0",
      //         "id": "2019-04-02",
      //         "kcqty": "51015",
      //         "rl": "29",
      //         "thQty": "0",
      //         "xsQty": "1"
      //       },
      //       {
      //         "SellTotal": "0",
      //         "YKC": "51020",
      //         "bdQty": "0",
      //         "cgQty": "0",
      //         "cgthQty": "0",
      //         "ckname": "",
      //         "count": "30",
      //         "dcqty": "0",
      //         "drqty": "0",
      //         "id": "2019-04-01",
      //         "kcqty": "51015",
      //         "rl": "30",
      //         "thQty": "0",
      //         "xsQty": "0"
      //       }
      //     ],       //数据，可以是数据，对象
      //     startRows: 11,//行列范围
      //     startCols: 6,
      //     minRows: 5,  //最小行列
      //     minCols: 5,
      //     maxRows: 20,  //最大行列
      //     maxCols: 20,
      //     rowHeaders: false,//列表头
      //     colHeaders:   [
      //       '序号', '时间', '销售金额', '销售数量', '调出数量','调入数量','调出调入仓库','其他变动数量','采购数量','库存数量'
      //     ],//自定义列表头or 布尔值
      //     // minSpareCols: 2, //列留白
      //     // minSpareRows: 2,//行留白
      //     currentRowClassName: 'currentRow', //为选中行添加类名，可以更改样式
      //     currentColClassName: 'currentCol',//为选中列添加类名
      //     autoWrapRow: false, //自动换行
      //
      //     contextMenu: {   //自定义右键菜单，可汉化，默认布尔值
      //       items: {
      //         "row_above": {
      //           name:'上方插入一行'
      //         },
      //         "row_below": {
      //           name:'下方插入一行'
      //         },
      //         "col_left": {
      //           name:'左方插入列'
      //         },
      //         "col_right": {
      //           name:'右方插入列'
      //         },
      //         "hsep1": "---------", //提供分隔线
      //         "remove_row": {
      //           name: '删除行',
      //         },
      //         "remove_col": {
      //           name: '删除列',
      //         },
      //         "make_read_only": {
      //           name: '只读',
      //         },
      //         "borders": {
      //           name: '表格线',
      //         },
      //         "commentsAddEdit": {
      //           name: '添加备注',
      //         },
      //         "commentsRemove": {
      //           name: '取消备注',
      //         },
      //         "freeze_column": {
      //           name: '固定列',
      //         },
      //         "unfreeze_column": {
      //           name: '取消列固定',
      //         },
      //         "hsep2": "---------",
      //       }
      //     },//右键效果
      //     fillHandle: true, //选中拖拽复制 possible values: true, false, "horizontal", "vertical"
      //     fixedColumnsLeft: 0,//固定左边列数
      //     fixedRowsTop: 0,//固定上边列数
      //     // mergeCells: [   //合并
      //     //   {row: 1, col: 1, rowspan: 3, colspan: 3},  //指定合并，从（1,1）开始行3列3合并成一格
      //     //   {row: 3, col: 4, rowspan: 2, colspan: 2}
      //     // ],
      //     readOnly: true,
      //     filters: true,
      //     dropdownMenu: true,
      //     columns: [     //添加每一列的数据类型和一些配置
      //       {data: 'rl'},
      //       {
      //         data: 'id',
      //       },
      //       {data: 'SellTotal'},
      //       {data: 'xsQty'},
      //       {data: 'dcqty'},
      //       {data: 'drqty'},
      //       {data: 'ckname'},
      //       {data: 'bdQty'},
      //       {data: 'cgthQty'},
      //       {data: 'kcqty'},
      //     ],
      //     manualColumnFreeze: true, //手动固定列
      //     manualColumnMove: true, //手动移动列
      //     manualRowMove: true,   //手动移动行
      //     manualColumnResize: true,//手工更改列距
      //     manualRowResize: true,//手动更改行距
      //     comments: false, //添加注释
      //     width: 880,
      //     height: 487,
      //     // fixedRowsBottom: 2,//固定下面两行
      //     cell: [
      //       {row: 1, col: 1, comment: {value: 'this is test'}}, //注释
      //     ],
      //     language: 'zh-CN',
      //     customBorders:[],//添加边框
      //     columnSorting: true,//排序
      //     stretchH: 'all',//根据宽度横向扩展，last:只扩展最后一列，none：默认不扩展
      //   },
      // }
    },

    mounted(){
      this.dataFn();
    },
    methods:{
      dataFn: function(){

      }
    }
  }
</script>


<!--<style src="../../node_modules/handsontable/dist/handsontable.full.css"></style>-->
