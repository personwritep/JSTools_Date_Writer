// ==UserScript==
// @name        JSTools Date Writer ▢
// @namespace        http://tampermonkey.net/
// @version        0.2
// @description        「スクリプトツール一覧表」に更新日付データを記入「Ctrl+Shift+F10」
// @author        Ameba Blog User
// @match        https://blog.ameba.jp/ucs/entry/srventryinsertinput.do*
// @match        https://blog.ameba.jp/ucs/entry/srventryupdateinput.do*
// @icon        https://www.google.com/s2/favicons?sz=64&domain=ameba.jp
// @grant        none
// @updateURL        https://github.com/personwritep/JSTools_Date_Writer/raw/main/JSTools_Date_Writer.user.js
// @downloadURL        https://github.com/personwritep/JSTools_Date_Writer/raw/main/JSTools_Date_Writer.user.js
// ==/UserScript==


let date_all=[]; // 一覧表の日付データの配列

let retry=0;
let interval=setInterval(wait_target, 100);
function wait_target(){
    retry++;
    if(retry>10){ // リトライ制限 10回 1sec
        clearInterval(interval); }
    let target=document.getElementById('cke_1_contents'); // 監視 target
    if(target){
        clearInterval(interval);
        main(); }}



function main(){
    let editor_iframe;
    let iframe_doc;

    let target=document.getElementById('cke_1_contents'); // 監視 target
    let monitor=new MutationObserver(catch_key);
    monitor.observe(target, {childList: true}); // ショートカット待受け開始

    catch_key();

    function catch_key(){
        editor_iframe=document.querySelector('.cke_wysiwyg_frame');
        if(editor_iframe){ // iframe がある「通常表示」の場合
            iframe_doc=editor_iframe.contentWindow.document;
            if(iframe_doc){
                iframe_doc.addEventListener("keyup", check_key); }

            function check_key(event){
                if(event.ctrlKey && event.shiftKey && event.keyCode==121){ //「Ctrl+Shift+F10」処理
                    event.preventDefault();
                    setTimeout(()=>{
                        write_table(); }, 100); } }
        } //「通常表示」の場合
        else{
        } //「HTML表示」の場合

    } // catch_key




    function write_table(){
        let links=iframe_doc.querySelectorAll('#ambt0 td:first-child a');

        if(links.length==date_all.length){ // 表データ数と日付データ数の一致を確認

            for(let k=0; k<links.length; k++){
                let table_tr=links[k].closest('tr');
                let target_td=table_tr.querySelector('td:last-child');
                if(target_td){
                    target_td.textContent=date_all[k]; }}

        }} // write_in()

} // main()




date_all=[
    "2021-11-02","2023-09-09","2023-11-15","2021-08-17","2023-12-15","2023-04-15",
    "2023-12-17","2023-12-22"]




/*
date_all=[
    "2023-12-18","2023-12-14","2023-07-03","2022-03-03","2022-08-25","2022-08-25",
    "2023-12-30","2022-04-19","2023-10-28","2023-08-23","2022-10-11","2023-10-27",
    "2021-03-14","2023-12-25","2023-05-31","2023-10-13","2022-09-16","2023-01-24",
    "2022-09-23","2022-07-27","2023-12-08","2019-12-25","2023-10-24","2023-08-02",
    "2023-08-05","2022-11-03","2022-11-04","2023-11-29","2023-05-20","2020-05-23",
    "2022-09-28","2023-12-20","2023-12-21","2023-12-04","2023-07-09","2023-08-25",
    "2023-08-25","2023-08-25","2023-08-25","2023-08-25","2023-08-25","2023-08-25",
    "2023-12-02","2023-12-02","2023-09-20","2023-09-16","2023-11-01","2023-03-31",
    "2021-08-23","2022-05-29","2023-11-03","2023-10-05","2022-07-21","2023-09-03",
    "2022-11-19","2022-11-21","2021-12-22","2023-02-24","2023-09-07","2022-09-06",
    "2023-12-31","2023-10-11","2023-12-15","2022-04-04","2023-11-14","2023-11-27",
    "2023-11-26","2023-10-10","2023-03-29","2023-08-26","2023-08-26","2023-07-26",
    "2023-10-23","2023-04-10","2023-04-12","2023-04-12","2021-01-28","2021-09-26",
    "2023-09-13"]
*/
